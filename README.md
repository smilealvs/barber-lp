# Lord 4L Barber

Site institucional de uma página para a barbearia Lord 4L — peça de portfólio desenvolvida como site estático, sem build e sem dependências de framework.

Identidade visual "Cadeira à Meia-Noite": fundo charcoal, tipografia editorial (Playfair Display + Inter) e um único acento dourado. O herói apresenta a marca animada da casa — um crânio com pompadour — em vídeo com fundo transparente.

## Tecnologias

- HTML, CSS e JavaScript puros — sem framework, bundler ou dependências de runtime.
- Google Fonts via CDN.
- Galeria do Instagram incorporada pelo widget Elfsight (região gerenciada pelo cliente).

## Estrutura

```
index.html
css/style.css
js/script.js
assets/
  favicon/        favicons + site.webmanifest
  images/         marca animada (.webm / .mp4), poster e imagem de compartilhamento
```

Seções: `#inicio` (herói), `#servicos`, `#galeria`, `#contato` e o rodapé.

## Como rodar

Não há etapa de build. Sirva a pasta como conteúdo estático e abra via `http://` (o vídeo e o manifest não funcionam corretamente em `file://`):

```bash
npx serve .
# ou
python -m http.server
```

## Detalhes técnicos

- **Vídeo com transparência:** o `.webm` é VP9 com canal alfa (`yuva420p`, ~1 MB), então a marca flutua sobre o painel sem caixa preta. O `.mp4` de fallback não suporta alfa, por isso tem o fundo assado na cor do painel. O vídeo toca em todas as larguras; como o Safari afirma reproduzir VP9 mas não decodifica, o `script.js` troca a fonte para o `.mp4` quando o primeiro quadro do webm não chega (Chrome e Android continuam no webm, com alfa real).
- **Acessibilidade:** HTML semântico, `aria-current` na navegação, `aria-hidden` no vídeo decorativo, foco visível e contraste AA.
- **Movimento reduzido:** `prefers-reduced-motion` desativa animações e pausa o vídeo.
- **Responsivo:** verificado de 320px a 1920px sem overflow horizontal; menu colapsa em 700px e o herói empilha em 900px.

## Conteúdo

Os dados da barbearia (serviços, preços, horário, endereço e contato) são reais e podem ser atualizados diretamente em `index.html`.
