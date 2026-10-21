---
name: Billy Proscia Renovations
description: Calm band system for a bathroom renovation crew. Call the pros, 718-400-WORK.
colors:
  paper: "#f6f5f2"
  card: "#ffffff"
  field: "#ebe8e3"
  ink: "#172131"
  body: "#2b3442"
  soft: "#4d5664"
  red: "#9c1d1a"
  deep: "#172131"
  on-dark: "#fbf8f6"
  on-red-soft: "#f6dcd8"
  on-deep-soft: "#cfd6e2"
  yellow: "#ffc629"
  yellow-2: "#ffd65c"
  focus: "#9c1d1a"
  error: "#b3261e"
typography:
  display:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(42px, 12vw, 80px)"
    fontWeight: 400
    lineHeight: 1.02
    letterSpacing: "-0.005em"
  headline:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(30px, 7.6vw, 48px)"
    fontWeight: 400
    lineHeight: 1.08
    letterSpacing: "-0.005em"
  title:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(21px, 5.8vw, 26px)"
    fontWeight: 400
    lineHeight: 1.15
  title-sm:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "18px"
    fontWeight: 400
    lineHeight: 1.2
  lede:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(17px, 4.6vw, 19px)"
    fontWeight: 400
    lineHeight: 1.7
  body:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.7
  label:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "14px"
    fontWeight: 400
    lineHeight: 1.4
rounded:
  field: "10px"
  card: "24px"
  pill: "999px"
spacing:
  gutter: "20px"
  gutter-wide: "40px"
  band: "64px"
  band-wide: "96px"
  gap-sm: "12px"
  gap-md: "20px"
  gap-lg: "32px"
  gap-xl: "64px"
components:
  button-primary:
    backgroundColor: "{colors.yellow}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  button-primary-hover:
    backgroundColor: "{colors.yellow-2}"
    textColor: "{colors.ink}"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.on-dark}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  input-text:
    backgroundColor: "{colors.field}"
    textColor: "{colors.ink}"
    rounded: "{rounded.field}"
    padding: "13px 14px"
    height: "52px"
  chip:
    backgroundColor: "{colors.field}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    padding: "0 18px"
    height: "48px"
  chip-selected:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.on-dark}"
  form-card:
    backgroundColor: "{colors.card}"
    rounded: "{rounded.card}"
    padding: "clamp(20px, 5vw, 32px)"
  step-badge:
    backgroundColor: "{colors.yellow}"
    textColor: "{colors.ink}"
    typography: "{typography.title-sm}"
    size: "48px"
  float-text:
    backgroundColor: "{colors.yellow}"
    textColor: "{colors.ink}"
    size: "60px"
---

# Design System: Billy Proscia Renovations

## Overview

**Creative North Star: "The Crew Shirt"**

The page is dressed like the two men who turn up at the door: shirt red, work-van navy, a hard-hat yellow that appears only where a hand should go. Full-width bands alternate between warm paper and the two dark colours, and the dark bands carry a faint diagonal line texture like a pressed work fabric. Nothing floats or layers; depth comes from the band changes, not from shadows.

Density is low and phone-first. Each band holds one heading, at most one supporting line, and one job (meet the crew, pick a service, see ideas, follow the steps, write the text, call). Type is a friendly rounded display face (Cal Sans) for everything a person would say out loud, including the phone number, set against a plain system body face for the reading text.

Motion is a short sequence: the hero headline lands letter by letter with a slight overshoot, content below the first screen rises 12px into place, and a yellow text circle slides up once the hero is gone.

**Key Characteristics:**
- Paper, red and navy bands; yellow is a fill, never a surface.
- Rounded, pill-shaped controls (999px) and soft 24px cards; no sharp corners on anything you touch.
- Cal Sans at weight 400 for headings, buttons, labels, service rows and phone numbers.
- Flat by default; two soft ambient shadows only.
- Dark bands wear the diagonal-line texture; paper bands are plain.

## Colors

Three grounds (paper, crew red, deep navy) and one hard-hat yellow that is always a fill.

### Primary
- **Crew-Shirt Red** (`red`): the crew's red shirts, deepened. The hero and closing "Call the pros." bands, the "Renovations" line of the wordmark, the header phone icon, the text caret, and (as `focus`) every hover and focus outline on light grounds.

### Secondary
- **Hard-Hat Yellow** (`yellow`): the one accent. Primary button fill, numbered step badges, the floating text circle, the arrow fill on hovered service rows, text selection, the focus outline on dark bands, and the accent phrase at the end of a heading on red or navy. Hover lightens to **Lit Yellow** (`yellow-2`).

### Tertiary
- **Work-Van Navy** (`deep`): the services band, the how-it-works band and the footer. The same value serves as **Ink** (`ink`), the heading and control-text colour on light grounds and the only text colour allowed on yellow.

### Neutral
- **Warm Paper** (`paper`): page ground, header, and the light bands (crew, ideas, form).
- **Card White** (`card`): the form card and the Facebook link card on paper.
- **Plaster** (`field`): input and chip backgrounds inside the white form card; also the placeholder fill behind images while they load.
- **Body Slate** (`body`): running text on light grounds.
- **Soft Slate** (`soft`): ledes, notes, placeholders, helper text.
- **On-Dark** (`on-dark`): headings, buttons and links on red and navy.
- **Blush** (`on-red-soft`) and **Mist** (`on-deep-soft`): running text on red and on navy respectively.
- **Error Red** (`error`): field error text and the border of an invalid field.

### Named Rules
**The Hard-Hat Rule.** Yellow is a fill or a mark on a dark ground. It never fills a band, never carries body text, and text sitting on it is always Ink. If yellow ever has to be text on a light ground, it drops to the darkened amber `#8a5a00` (5.4:1), not the raw yellow.

**The Two-Outline Rule.** Interactive outlines are 3px and offset. On light grounds they are Crew-Shirt Red; on red, navy, the hero and the footer they switch to Hard-Hat Yellow. Yellow never outlines a yellow fill on light ground.

**The Accent-Phrase Rule.** On red and navy bands, the last phrase of a heading may be set in yellow ("built by the pros.", "renovate.", "works."). Paper-band headings stay all Ink.

## Typography

**Display Font:** Cal Sans (with Avenir Next, Segoe UI, system-ui)
**Body Font:** system UI stack (-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial)

**Character:** A round, chunky, friendly display face that reads like signage on a work van, paired with the phone's own UI font so reading text feels native inside Facebook's in-app browser.

### Hierarchy
- **Display** (400, `clamp(42px,12vw,80px)` on phones, `clamp(42px,7vw,96px)` from 760px, 1.02): the hero H1 only, max 11ch on phones; from 760px the accent phrase drops to its own line.
- **Headline** (400, `clamp(30px,7.6vw,48px)`, 1.08, -0.005em, balanced wrap): every section H2.
- **Title** (400, `clamp(21px,5.8vw,26px)`, 1.15): service rows and the Facebook link card (19-22px); step titles at 21px (22px from 1024px).
- **Title-sm** (400, 18px, 1.2): buttons, form labels and legends, the header phone number (20px from 760px), step badge numerals (20px).
- **Lede** (400, `clamp(17px,4.6vw,19px)`, max 40ch, Soft Slate): one supporting line under a section heading. The hero promise is the same role at `clamp(17px,4.7vw,20px)`/1.5, max 32ch (40ch from 760px).
- **Body** (400, 16px, 1.7): running text, inputs, chips, errors, footer.
- **Label** (400, 14px): notes, helper text such as "(optional)", the eyebrow, the line under the form button.

### Named Rules
**The Say-It-Out-Loud Rule.** Anything a person would speak (headings, button labels, service names, field questions, the phone number) is Cal Sans at 400. Anything they would read quietly (paragraphs, inputs, notes) is the system face. Cal Sans is never bolded.

**The Number-Is-the-Brand Rule.** The phone number is set as display type wherever it appears as a target: header (18-20px), close band (`clamp(34px,10vw,56px)`), with the plain digits under the vanity number in body type.

## Layout

A single centered column (max 1160px) with a 20px gutter on phones and 40px from 760px. Sections are full-bleed bands with 64px vertical padding, 96px from 760px; the hero uses 56/64px, then 96/112px.

Phone-first, stacked. Breakpoints:
- **760px:** wider gutter and band padding, hero buttons sit side by side (min 240px each), the ideas grid becomes three equal columns.
- **1024px:** the crew band splits 1fr/1fr with the photo on the right; service rows become two columns with a 64px column gap; the form band splits 1fr/1.2fr with the heading sticky at 40px from the top; the close band puts the heading and the big phone number on one baseline row; steps become three columns.
- **380px and below:** chips tighten to 14px side padding.

Rhythm: 12px between sibling controls and grid images (20px on desktop), 16-20px inside heading groups and form fields, 28-36px between a heading and its content, 64px between columns at desktop. Text blocks cap at 640px; the form at 600px; the Facebook card at 520px; images at 440px in the crew band.

Images are 4:5 portrait, cropped with object-fit, rounded to the card radius. On phones the first idea image spans the full width above a pair.

## Elevation & Depth

Flat. Depth comes from alternating bands (paper, red, navy) and from white cards sitting on paper, not from shadows. The dark bands carry a fabric-like diagonal line texture (a 1px line of white at 3.5% every 23px at 135deg), which is the world's own material; paper bands stay plain.

### Shadow Vocabulary
- **Card lift** (`box-shadow: 0 8px 24px rgba(23,33,49,.08)`): a white link card on paper, so it reads as tappable. It does not change on hover.
- **Float** (`box-shadow: 0 10px 28px rgba(23,33,49,.3)`): only the fixed floating text circle, which sits over content.

### Named Rules
**The Band-Not-Shadow Rule.** A new section gets its separation from a band colour change, never from a shadow or a border box. Shadows are reserved for the two roles above.

## Shapes

Soft and round everywhere a hand goes. Three radii: 10px for text inputs, 24px for cards and photos, 999px pills for buttons and chips. Circles (50%) for the service-row arrows (44px), the step badges (48px) and the floating text circle (60px). Borders are 2px and transparent at rest so hover, focus and error states can colour them without shifting layout. The only dividers are 1px hairlines between service rows on navy (white at 12%).

## Components

### Buttons
Big, round, thumb-sized.
- **Shape:** full pill (999px), 56px tall, 26px side padding, Cal Sans 18px, optional 20px leading icon.
- **Primary:** Hard-Hat Yellow fill with Ink text and a matching yellow border. Inside the form it stretches full width.
- **Ghost:** transparent with On-Dark text and a 2px border at 75% On-Dark, for use on red and navy only.
- **Hover (pointer devices only):** primary lightens to Lit Yellow; ghost firms its border to white and adds a 10% white wash; the form's submit button gains a 3px red outline. Colour transitions run 0.2s.
- **Press:** scale to 0.98 over 0.12s.
- **Focus:** 3px outline offset 3px (red on light, yellow on dark).

### Chips
- **Style:** single-choice radio chips, Plaster fill, Ink body text 16px, 48px tall, pill radius, 2px transparent border.
- **State:** hover gives a red border; selected inverts to Ink fill with On-Dark text; invalid gives every chip an Error Red border; keyboard focus draws a red outline on the label.

### Cards / Containers
- **Corner Style:** 24px.
- **Background:** Card White on paper.
- **Shadow Strategy:** form card is flat; the Facebook link card uses Card lift.
- **Internal Padding:** `clamp(20px,5vw,32px)` for the form; 14px 16px 14px 22px for the link card.

### Inputs / Fields
- **Style:** Plaster fill, 2px transparent border, 10px radius, 52px min height (110px for textareas, vertical resize), body type in Ink, red caret.
- **Labels:** Cal Sans 18px question phrasing above the field; "(optional)" in 14px Soft Slate.
- **Focus / Hover:** border turns Crew-Shirt Red (0.15s); no glow.
- **Error:** border and a 16px message in Error Red, shown under the field only while invalid.

### Navigation
- **Header:** paper, 64px tall (76px from 760px). Two-line wordmark at left: "Billy Proscia" in Cal Sans 20px (24px from 760px) over "RENOVATIONS" in 11px uppercase, 0.14em tracking, Crew-Shirt Red. Phone number at right in Cal Sans with a red phone icon; it turns red on hover. No menu.
- **Footer:** navy with texture, 16px Mist text, On-Dark links that turn yellow on hover, 44px min tap height, extra bottom padding to clear the floating circle.

### Service Rows (signature)
Full-width link rows on navy, Cal Sans title on the left and a 44px round arrow on the right, separated by hairlines, 76px minimum height. The row itself never changes colour; only the arrow does, filling yellow with an Ink arrow on hover or focus. Each row pre-selects the matching chip in the form.

### Numbered Steps (signature)
A 48px yellow circle holding a Cal Sans numeral, beside a Cal Sans step title in On-Dark and one Mist sentence. Stacked on phones, three columns from 1024px.

### Floating Text Circle (signature)
One 60px yellow circle, fixed 16px from the bottom-right safe area, holding a 26px chat icon, with the Float shadow. It slides up (0.35s, `cubic-bezier(.2,.8,.2,1)`) once the hero leaves view and slides away while the form is on screen. It is a circle, never a bottom bar, and it is absent without JavaScript.

### Motion
- **Headline bounce-in:** hero H1 only. Each letter slides in from 50px right over 1s on `cubic-bezier(.34,1.56,.64,1)`, 20ms apart, after waiting up to 400ms for Cal Sans; the plain heading is restored when the last letter lands.
- **Rise:** content that starts below the first screen fades up 12px over 0.4s ease-out as it enters. Content already on screen never animates.
- **Reduced motion:** all of the above, smooth scrolling and button transitions switch off.

### Eyebrow (present by owner decision; do not extend)
A quiet 14px pill with a 7px yellow dot, Ink on a 6% Ink wash (On-Dark on 13% white on dark grounds), marked up as a paragraph, not a heading. The build carries two: above the hero H1 and above the form heading. Ellie chose these on 2026-10-19 against Impeccable's craft-floor ban; they are recorded here so they stay quiet (no arrow, hover, shadow or full yellow fill), not as a pattern to add to new headings.

## Do's and Don'ts

### Do:
- **Do** alternate full-bleed bands of Warm Paper, Crew-Shirt Red and Work-Van Navy, and put the diagonal line texture on the red and navy bands only.
- **Do** keep text on yellow in Ink, and use the amber `#8a5a00` if yellow ever has to be text on a light ground.
- **Do** set headings, buttons, labels, service names and the phone number in Cal Sans 400, and running text in the system face at 16px/1.7.
- **Do** make every control at least 44px tall (buttons 56px, inputs 52px, chips 48px).
- **Do** use pill radius (999px) for buttons and chips, 24px for cards and photos, 10px for inputs.
- **Do** put hover styles inside a `(hover:hover)` query so taps don't leave them stuck on, and switch outlines from red to yellow on dark grounds.
- **Do** honour reduced motion by disabling the bounce-in, the rise, the float slide and button transitions.

### Don't:
- **Don't** fill a band, card or large surface with yellow; it is a fill for buttons, badges, the arrow state and the floating circle only.
- **Don't** separate sections with shadows or bordered boxes; change the band colour instead.
- **Don't** add a third shadow role or a hover shadow change on cards.
- **Don't** bold Cal Sans.
- **Don't** turn the floating text circle into a bottom bar or add a second floating control.
- **Don't** add eyebrows to more headings.
