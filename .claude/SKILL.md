# Honeycomb Academy — Brand & Design Skill

## When to use this skill
Read this file before generating any visual output — comics, slides,
diagrams, layouts, UI mockups, or components. Apply everything below
automatically without prompting the user to confirm.

---

## Behavioral Instructions

Always:
- Use the layout system defined below
- Load all assets from the jsDelivr URLs in the Asset Library
- Import Poppins and Roboto from Google Fonts on every HTML file
- Select character assets based on emotional context (see Asset Library)
- Build all layouts as self-contained HTML files
- Apply visual tone: flat, quiet, editorial

Never:
- Use raw.githubusercontent.com URLs — they will not render
- Use pure black or near-black as a background
- Use gradients, drop shadows, or blur effects
- Use the default Claude diagram style (gray boxes, blue arrows)
- Leave assets out when contextually appropriate
- Truncate output — always write complete files

---

## Brand Colors

Cobalt (primary background):   #0278CD
Denim (card background):        #01487B
Royal (nested card/input):      #0160A4
Slate (caption bars, text):     #25303E
Honey (numbers, accents):       #FFB000
Amber (callout background):     #F8AD00
Light Blue (secondary text):    #93D1F2
Pacific (borders, links):       #0298EC
White:                          #FFFFFF

Text on dark:   #FFFFFF (primary), #93D1F2 (secondary)
Text on Amber:  #25303E

---

## Typography

Always include this import at the top of every HTML file:
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@600;700&family=Roboto:wght@400;500&display=swap');

Poppins 700:   Headlines, panel numbers, callout numbers
Poppins 600:   Card titles, labels, tags, wordmarks
Roboto 500:    UI labels, emphasized body
Roboto 400:    Captions, body copy, secondary text

Scale:
- Headline:       26-28px Poppins 700 #FFFFFF
- Card title:     12-13px Poppins 600 #FFFFFF
- Card body:      11-12px Roboto 400 #93D1F2
- Caption:        10-11px Roboto 400 italic #93D1F2
- Panel number:   13px Poppins 700 #FFB000
- Tag:            10px Poppins 600 uppercase letter-spacing 2.5px #FFB000

---

## Layout System

Outer container:
  background: #0278CD
  border-radius: 16px
  padding: 24-32px

Primary cards:
  background: #01487B
  border-radius: 12px
  overflow: hidden

Nested UI cards (screen mockups, inputs):
  background: #0160A4
  border-radius: 8-10px

Caption bars:
  background: #25303E
  padding: 8-10px 12-14px
  font: 10-11px Roboto 400 italic
  color: #93D1F2

Callout bar:
  background: #F8AD00
  border-radius: 10px
  padding: 14px 18px
  display: flex, align-items: center, gap: 14px
  text: 12px Roboto 500 color #25303E

Card grid:
  display: grid
  grid-template-columns: repeat(3, 1fr) or repeat(2, 1fr)
  gap: 10-12px

Loading indicator:
  Three circles in #FFB000 at opacity 0.9 / 0.6 / 0.3

Canvas hex mark (always use this exact SVG):
  <svg viewBox="0 0 14 14" width="14" height="14">
    <polygon points="7,1 12,4 12,10 7,13 2,10 2,4" fill="#FFB000"/>
  </svg>

Canvas UI pattern:
  Top bar: #0160A4 bg + hex mark + "Canvas" Poppins 600 #93D1F2
  Input: #0160A4 bg, border 1.5px #0298EC, border-radius 8px,
         white text, #FFB000 send button

---

## Comic Format

Panel structure:
  .panel-scene   — colored bg (#01487B or #0160A4) + assets + UI mockups
  .panel-caption — #25303E bar, Roboto 400 italic, #93D1F2 text

Grid: 3 columns default
Panel numbers: Poppins 700 13px #FFB000 top-left absolute

Character sizing:
  Hero:        72px
  Supporting:  52-64px
  Ambient:     36-44px
  Inactive:    opacity 0.4-0.5 + filter: brightness(0.5) saturate(0.3)

UI mockups inside panels: #0160A4 nested cards, #FFB000 accents
Darkest panel background: #01487B — never pure black

Visual tone:
  Flat, clean, editorial — not cartoonish
  Stress is quiet — no fire, explosions, PANIC text, red alerts
  Posture and composition carry emotion, not expressions
  Generous whitespace always

---

## Slide Format

Header: left = tag + title + subtitle, right = hero asset 100-120px
Cards: 2-3 col grid, #01487B bg, asset icon 44px + title + body
Callout: #F8AD00 bar, icon 38px + Roboto 500 text #25303E
People row: 2-4 person assets 52-64px, bottom-right, flex-end

---

## Asset Library

Base URL: https://cdn.jsdelivr.net/gh/midgepickett/honeycomb-academy-assets@main/assets/
IMPORTANT: Always use this jsDelivr URL. Never use raw.githubusercontent.com.

### Characters

Person 01 — square head, blue/gold:
https://cdn.jsdelivr.net/gh/midgepickett/honeycomb-academy-assets@main/assets/HNY_Academy-Person_01.png
Use for: neutral, default engineer state

Person 02 — diamond head, all blue:
https://cdn.jsdelivr.net/gh/midgepickett/honeycomb-academy-assets@main/assets/HNY_Academy-Person_02.png
Use for: focused, analytical, investigative

Person 03 — star-burst head, gold/blue:
https://cdn.jsdelivr.net/gh/midgepickett/honeycomb-academy-assets@main/assets/HNY_Academy-Person_03.png
Use for: energized, engaged, breakthrough moment

Person 04 — hex head, blue/gold:
https://cdn.jsdelivr.net/gh/midgepickett/honeycomb-academy-assets@main/assets/HNY_Academy-Person_04.png
Use for: alert, on-call, reactive

### Mascots

Small Bee:
https://cdn.jsdelivr.net/gh/midgepickett/honeycomb-academy-assets@main/assets/HNY_Academy-Small_Bee.png
Use for: ambient presence, waiting, quiet moments

Big Bee + Flower:
https://cdn.jsdelivr.net/gh/midgepickett/honeycomb-academy-assets@main/assets/HNY_Academy-Big_Bee_Flower.png
Use for: hero image, covers, feature slides

### Icons

Hive:
https://cdn.jsdelivr.net/gh/midgepickett/honeycomb-academy-assets@main/assets/HNY_Academy-Hive.png
Use for: team, collaboration, shared knowledge

Magnifying Glass:
https://cdn.jsdelivr.net/gh/midgepickett/honeycomb-academy-assets@main/assets/HNY_Academy-Magnifying_Glass.png
Use for: search, investigation, query context

Trace Waterfall:
https://cdn.jsdelivr.net/gh/midgepickett/honeycomb-academy-assets@main/assets/HNY_Academy-Trace_Waterfall.png
Use for: Canvas results, tracing, observability output

Thumbs Up:
https://cdn.jsdelivr.net/gh/midgepickett/honeycomb-academy-assets@main/assets/HNY_Academy-Thumbs_Up.png
Use for: success, resolution, pro tips

OTel Telescope:
https://cdn.jsdelivr.net/gh/midgepickett/honeycomb-academy-assets@main/assets/HNY_Academy-Otel_Telescope.png
Use for: observability, monitoring, looking deeper

Experiment (flask):
https://cdn.jsdelivr.net/gh/midgepickett/honeycomb-academy-assets@main/assets/HNY_Academy-Experiment.png
Use for: testing, iteration, hands-on activities

Autonomy:
https://cdn.jsdelivr.net/gh/midgepickett/honeycomb-academy-assets@main/assets/HNY_Academy-Autonomy.png
Use for: independence, self-service, empowerment

Handshake:
https://cdn.jsdelivr.net/gh/midgepickett/honeycomb-academy-assets@main/assets/HNY_Academy-Handshake.png
Use for: collaboration, partnership, onboarding

Mountain:
https://cdn.jsdelivr.net/gh/midgepickett/honeycomb-academy-assets@main/assets/HNY_Academy-Mountain.png
Use for: advanced topics, goals, aspirational content

Funnel:
https://cdn.jsdelivr.net/gh/midgepickett/honeycomb-academy-assets@main/assets/HNY_Academy-Funnel.png
Use for: filtering, narrowing, query refinement

Flower:
https://cdn.jsdelivr.net/gh/midgepickett/honeycomb-academy-assets@main/assets/HNY_Academy-Flower.png
Use for: growth, learning, positive outcomes

Sun:
https://cdn.jsdelivr.net/gh/midgepickett/honeycomb-academy-assets@main/assets/HNY_Academy-Sun.png
Use for: clarity, insight, illumination