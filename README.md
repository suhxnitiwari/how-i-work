# How I Work

*How I work, measured three ways: my DISC style, my top five CliftonStrengths and my RIASEC code, each tied to real work.*

**Live:** https://suhxnitiwari.github.io/how-i-work/

Part of my portfolio at [suhanitiwari.com](https://suhanitiwari.com).

## What it is

A one-page "user manual" for working with me, built from three assessments:

- **DISC:** my primary style (D, Dominance) on a quadrant wheel, with what motivates me, how I communicate and how to work with me, plus six flip cards that each pair a trait with a real scenario and its result, including the one I'm still working on.
- **CliftonStrengths:** my top five (Relator, Empathy, Individualization, Developer, Communication), each with how it shows up at work, and a short slideshow on how the two domains they fall in work together.
- **RIASEC:** my Holland code (Artistic, Social, Enterprising) on a hexagon of all six scores.

## How it's built

- **Data-accurate SVG charts.** The RIASEC hexagon is hand-built SVG where each point's distance from the center equals its score, drawn over concentric guide rings. Each point is keyboard-focusable with a `<title>` tooltip, and the whole figure has an `aria-label` listing all six scores for screen readers. The DISC wheel is four SVG arc paths with my quadrant highlighted.
- **Accessible tabs.** The three tests switch as an ARIA tablist with roving `tabindex` and arrow-key navigation, and links can deep-link straight to a test (`#disc`, `#strengths`, `#riasec`).
- **CSS 3D flip cards** using `perspective`, `rotateY` and `backface-visibility`, toggled through `aria-pressed` so their state is exposed to assistive tech, with visible focus styles and a reduced-motion fallback.
- **A linked slideshow.** As you page through the CliftonStrengths summary, a bar above it lights up the matching strengths: the four Relationship Building themes, then the Influencing one, then all five together.
- **Shared site touches.** The gold sparkle cursor shared with my other pages ([`js/sparkle.js`](js/sparkle.js)) runs here too: only with a real mouse, and its glitter trail is skipped for reduced motion.

## Design choices

- Every trait is backed by a story. The flip cards follow a "when this happens, I do this" format, and the back of each one gives the scenario and the result.
- It's honest about the rough edges: the last DISC card is "Where I'm still growing."
- The voice is human, not résumé-speak. The CliftonStrengths section is subtitled "A suspicious amount of Relationship Building for someone with a very exclusive inner circle."

## Tech stack

HTML, CSS and vanilla JavaScript with inline SVG, no framework. Hosted on GitHub Pages.

CliftonStrengths® and each theme name are trademarks of Gallup, Inc.

## Ownership

© 2026 Suhani Tiwari. **All rights reserved.** The code is public so you can see how I build, not so you can reuse it. See [LICENSE](LICENSE).

Built by [Suhani Tiwari](https://suhanitiwari.com).
