# 4Site × Avalon capabilities site

Guidance for Claude Code and anyone new to this repo.

## What this is

A single-page capabilities site built for the partner agency Avalon, drawn from 4Site's branded capabilities deck. It is sent to Avalon before a call so they can pick the two or three topics they most want to see, and it doubles as the visual during the walkthrough.

Live page: https://4site-interactive-studios.github.io/avalon-dog-and-pony/

## Files

- `index.html` is the whole site. All HTML, CSS, and one small progressive-enhancement script live in this single file at the repo root. It references images from `assets/img/`.
- `assets/img/` holds the images, named by role (`hero_art`, `flower`, `shot_cart`, `logo_peta`, and so on).
- `README.md` is the public, client-facing repo readme.
- `avalon-dog-and-pony-demo-plan.md` is the internal plan behind the page: the content spec, the real numbers, the demo links, code-ownership notes, presenter assignments, and what was cut. It is internal only and not part of the published site.

Start with `avalon-dog-and-pony-demo-plan.md` for any question about content, figures, or why a card exists. It is the source of truth behind the page.

## Brand

- Colors: blue `#276DF0`, orange `#F97503`, deep navy `#241634`, yellow `#FAB713`.
- Type: Fraunces for display, Plus Jakarta Sans for body.
- Look: pastel section bands, clipped-corner panels, a carnival illustration theme.

## Writing voice

Plain and direct. No em-dashes. No marketing filler such as seamless, leverage, robust, foster, or showcase. Headings are sentence case. Let the real numbers do the work instead of adjectives.

## Content rules

- The page is Avalon-facing. Internal notes stay in the plan doc, never on the page.
- The copy and every figure are final and verified. The PETA and NWF/RAN stats are real. Do not change a number without checking the plan doc.
- The PETA recovery-logs link is a deliberate placeholder until the real one is dropped in.
- Presenter chips are initials plus a brand color: Bryan blue, Stef orange, Sydney yellow.

## Implementation notes

- Everything is in `index.html`. There is no build step. Open the file or serve the folder to preview.
- All content is visible without JavaScript. The fade-ins are enhancement only, gated on a `.js` class and turned off under `prefers-reduced-motion`.
- Images are served at 2x to every device. Screenshot cards (`shot_*`) are 1100px wide. The one exception is the Amnesty lightbox shot (`shot_lightbox`), which the deck only had at 317px, so it is effectively 1x.
- In the footer, the carnival illustration is clipped at the divider line by a full-bleed background band (`.footer-foot::before`), so it never shows below the line. Keep that band if you rework the footer.
- The repo is set up for GitHub Pages. A `.nojekyll` file is expected for Pages but is not in the repo yet; add one if Jekyll processing ever causes trouble.

## Standards

The 4site-standards skill, if installed, covers the writing, deliverable, and code-review standards used here.
