# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Stack

Static HTML/CSS/JS single-page site. No build tools or framework.

## Users

Men in the Guarulhos, SP region seeking a premium barbershop experience. They want to discover services, check prices and location, see the work, and book via WhatsApp.

## Product Purpose

Single-page website for Lord 4L Barber that presents the barbershop's identity, services, gallery, and contact — converting visitors into booked appointments via WhatsApp.

## Positioning

Premium personalized experience — no-rush service, attention to detail, and personal style — at competitive, accessible prices. The combination of care and affordability is what neighboring barbershops cannot truthfully copy.

## Operating Context

- Static single-page site (HTML/CSS/JS, pt-BR)
- Booking via WhatsApp (wa.me link), reached through a single CTA in the contact section
- Gallery is a client-managed Instagram feed embedded through Elfsight (a protected region, not editable here)
- Google Maps embed for location, with the address also linked as the fallback
- Animated logo mark in the hero (assets/images/lord4l-animated.webm — 1280×1500 VP9 with an alpha channel, ~1.0 MB — with an .mp4 fallback whose background is baked to the panel Ground); the video plays at every width, and script.js swaps to the .mp4 when the webm's first frame does not arrive (Safari), over the matching transparent still (assets/images/lord4l-still.webp, 1024×1200) as its poster

## Capabilities and Constraints

- Services and prices (subject to update):
  - Corte — R$ 40,00
  - Barba — R$ 40,00
  - Corte e barba — R$ 70,00
  - Progressiva — a partir de R$ 70,00
  - Relaxamento — a partir de R$ 30,00
  - Luzes — a partir de R$ 100,00
  - Sobrancelha — R$ 10,00
  - Depilação nasal/ouvido — R$ 10,00
  - Pézinho — R$ 10,00
- Hours: Monday to Saturday, 10:00–20:00
- Address: R. Elias Acras, 106 - Vila São Jorge, Guarulhos - SP, 07114-370
- Phone: (11) 2382-4280
- Instagram: @lord.4l
- Tone of voice: relaxed, informal, close to the audience
- Must preserve: prices, hours, location, and tone of voice

## Brand Commitments

- Name: Lord 4L Barber
- Tone: descontraído
- Dark theme: charcoal ground, warm ivory text, one muted gold accent, Playfair Display over Inter ("Cadeira à Meia-Noite")
- The shop's logo mark appears beside the wordmark in the header

## Evidence on Hand

- Animated brand logo (assets/images/lord4l-animated.webm / .mp4) and the still lifted from it (assets/images/lord4l-still.webp)
- Instagram feed (@lord.4l)
- Favicon and logo mark assets (assets/favicon/)

## Product Principles

1. Premium experience without the premium price
2. Personal attention and individual style
3. Frictionless booking via WhatsApp

## Accessibility & Inclusion

- Focus-visible styles on all interactive elements
- Semantic HTML structure
- Responsive design (mobile-first breakpoints)
- Reduced motion support via prefers-reduced-motion
