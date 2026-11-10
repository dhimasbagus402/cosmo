# Cosmo site: design direction

For `docs/` (the landing page, privacy page and share page). Read this before changing how the site looks.

Dial: ENERGY 2 / RHYTHM 2 / MOTION 2

## Identity

- **The night sky.** Cosmo is named for it, so the dark theme has a field of slow stars with the odd meteor. This is the motif. It stays, and nothing else gets added on top of it.
- **The island.** The product is a black island hanging from the top of a desktop. Every screenshot sits on a small "stage" so the island has something to hang from. Screenshots are real captures from the app, never mock-ups.

## Colour

- Accent: Cosmo orange `#ff9f0a`, the app's own default accent. It goes on the primary button, the one coloured word in the headline, feature labels and ticks.
- Sky indigo: in the stage corners, the hero desktop picture and the aurora.
- Neutrals: near-black `#050506` (dark) and warm paper `#f6f4f0` (light).
- No other hues. The swatches under Themes let a visitor try other accents, but the page itself stays orange.
- Text has to pass WCAG AA in both themes, including where it passes over the aurora's strongest tint. In light mode, orange text uses the darker `--accent-text` (`#9a4800`), never the raw accent.

## Type

Segoe UI Variable, the typeface Windows itself uses, because Cosmo is a Windows app and should look at home there. Headings use Display at weight 700 with tight tracking. Labels are sentence case, never uppercase with wide tracking.

## Layout

- Feature rows alternate sides. Music leads with the widest picture. Smaller features are paired side by side, and features without a screenshot yet are text blocks separated by a rule.
- Cards only where each item is a separate thing to click or read (install steps, support links, privacy notes).
- Below 820px the section links and the theme picker move into a labelled Menu. Every control is at least 44px on touch screens.

## Motion

- Motion is allowed where it shows how Cosmo behaves: the hero island opening into its pages, and islands dropping into their stages as they scroll in. The sky drifts.
- One-shot motion that sets the reading pace: the hero comes in piece by piece on load, each block slides in once as it scrolls into view, and the numbers count up once.
- The aurora (a violet and an orange light drifting slowly behind the page) stays by the owner's choice. It is the background's only movement in the light theme, where the stars are hidden. Recorded as a kept exception to antislop R-01/R-19 on 2026-11-10.
- Nothing else loops. No shimmer, glow pulses, floating or spinning.
- The Pause button stops the hero, the stars and the aurora. `prefers-reduced-motion` turns all motion off.

## Glow

There is one glow: the warm light under the island in the hero. Buttons, cards and icons stay flat.
