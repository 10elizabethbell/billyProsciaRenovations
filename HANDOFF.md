# Billy Proscia Renovations — handoff at ~60%

**Live:** https://10elizabethbell.github.io/billyProsciaRenovations/ · **Repo:** https://github.com/10elizabethbell/billyProsciaRenovations · **Built:** 2026-10-21 from Muse brief of 2026-10-21 (thin brief)

## What's built
- One page, calm band style: paper header (wordmark left, **718-400-WORK** tap-to-call top right) → red textured hero → crew photo → services rows on deep navy → "Ideas for your bathroom" (3 generated examples) + big Facebook link → How it works on navy → text-composing form → red close with "Call the pros." and the number → navy footer.
- Palette from the crew's shirts and the hard-hat logo on them: shirt red deepened to `#9c1d1a` (hero, close), deep navy `#172131` (services, how, footer), hard-hat yellow `#ffc629` as the one fill accent, `#8a5a00` when yellow must be text on light. Paper `#f6f5f2` (slightly warm to sit with the red).
- Hero is the plain textured red band. The only real photo (Facebook profile, 718×720 square) can't fill a wide desktop band without upscaling 2× and losing the men, so it sits in its own "crew at your door" section instead.
- Motion: H1 letter bounce-in, `.rise` fade-up, floating text circle (shows after the hero, hides over the form). All off under reduced motion; content visible without JS.
- Contact: hero "Plan my bathroom" (to the form) and "Text us" (`sms:`), service rows pre-select the matching chip, form composes a text and shows the call number as a fallback after submit, floating circle texts. No email anywhere (none exists).
- `og.png` (1200×630, red with the crew photo), `favicon.svg` / `apple-touch-icon.png` from "BP" lettering (no logo file).

## Assumptions I made
- **Voice "we":** the profile photo shows two people in company shirts. Which one is Billy is unknown, so the page never says "Billy" except in the business name.
- **Services list** (Full bathroom remodels, Walk-in showers, Tubs and tub-to-shower, Tile floors and walls, Vanities and fixtures) is inferred from "Bathroom renovation". Only that phrase is verbatim. No plumbing/electrical claims (licensing).
- **Copy promises** — "We show up when we say we will, treat your house with respect, and haul the old bathroom away ourselves", "We come and see it… give you a price", "the mess leaves with us": inferred from the dumpster in their photo and normal practice. Owner should confirm or rewrite.
- **Texting:** brief says "Accepts texts: unknown". The page leans on `sms:` (calm style); every text path falls back to the call number. If the number is a landline, swap "Text us" for the form button only and turn `CONFIG.FLOAT` off.
- **Header shows 718-400-WORK** (their brand) rather than digits; the close and footer spell out 718-400-9675.
- **Facebook link** is the vanity URL from the page's own metadata, `facebook.com/BillyBATS333` (the brief had the profile.php id; same page).
- **Form eyebrow "Winter is for inside jobs"** uses Muse's winter hook; it makes no scheduling claim.

## Placeholders and gaps
- **No place in the H1** (calm style wants one): the brief says do not publish a location. 718 = NYC, but they posted in NJ groups (Middlesex County). Add the area once the owner confirms it.
- **No real bathroom photos.** "Ideas for your bathroom" uses 3 generated images, labelled on the page as examples. Replace them with real jobs from Facebook first thing.
- No logo file (wordmark + "BP" favicon). The yellow hard-hat logo on their shirts is the obvious mark; get the file.
- No email, hours, reviews, prices, licence, years in business.

### Images
| File | Shows | Source | Licence |
|---|---|---|---|
| img/crew.webp | Two crew members in red company shirts by a dumpster | Facebook profile photo (og:image of facebook.com/BillyBATS333), fetched 2026-10-21, cropped 480×600 | Owner's own public photo; ask before keeping |
| img/idea-shower.webp | Glass walk-in shower, white tile, grey hex floor, brick wall | generated with gpt-image-1, 2026-10-21 ("real-estate photograph of a renovated small bathroom in a brick row house… walk-in shower…") | generated; OpenAI terms assign output to the user |
| img/idea-tub.webp | White alcove tub, sage vertical tile, oak floating vanity | generated with gpt-image-1, 2026-10-21 ("renovated family bathroom: white alcove bathtub… sage green subway tile…") | generated; OpenAI terms assign output to the user |
| img/idea-vanity.webp | Navy double vanity, white tile, black-and-white patterned floor | generated with gpt-image-1, 2026-10-21 ("navy blue double vanity… patterned cement floor tile… skylight") | generated; OpenAI terms assign output to the user |

## Questions for the owner
1. Which towns do you work in? (goes in the H1 and close)
2. Does 718-400-9675 take texts?
3. Can we use photos of your finished bathrooms (and any before/afters)?
4. Is it you and your son / partner in the photo, and what are your names? (A named owner builds trust.)
5. Besides bathrooms, what else do you take on (kitchens, basements, general contracting)? Facebook lists you as "general contractor".
6. Licence number / insured? Email for the footer? Hours?

## Ideas not built (yours to pick)
- **Crew photo in the hero on desktop** (like `og.png`): the desktop hero has a lot of empty red on the right; a 2-column hero with the crew card would fill it. Phone stays as is.
- **Before/after sliders** once real pairs exist (taste §4).
- **Opt-in signature motion — worlds from the trade:** (1) *tile being laid*: a grid of tiles snapping into place along the hero's bottom edge, grout lines drawing in, pushing apart under the finger (best fit); (2) shower water: droplets running down a glass pane you can wipe clear; (3) demo dust settling and being swept; (4) a level bubble that tilts with the pointer; (5) caulk bead drawn along a seam.
- Red vs navy: if the red hero reads too loud for Ellie, swap `--red` roles to navy and keep red only for the header "RENOVATIONS" and the phone icon.
- HOUSE-STYLE CONFLICTS (kept on purpose): Impeccable's detector flags the repeating-gradient band texture; eyebrows are a craft-floor ban. Both are Ellie's calm-style choices.

## Not verified
- Real-device tap/scroll, real SMS handoff on iOS and Android (body decoding checked in Chromium/WebKit by intercepting the composed URL).
- Facebook in-app browser behaviour of `sms:` links.
- Whether the profile photo is OK to publish on a website (it's public on their page).
