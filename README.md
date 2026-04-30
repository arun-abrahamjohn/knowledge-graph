# Technology · Power · Futures

An interactive knowledge graph mapping key concepts in the philosophy of technology — from Heidegger's enframing to democratic imagination, adversarial design to foreclosed futures.

## Using the graph

| Action | How |
|--------|-----|
| Pan | Click and drag |
| Zoom | Ctrl/Cmd + scroll, or pinch on trackpad |
| Focus a node | Click it — connected nodes highlight, others fade |
| Dismiss focus | Click the background or the focused node again |
| Search | Type in the search box (top right) |
| Reset | Click **Reset** in the toolbar |
| Guided tour | Click **Story mode** — steps through 22 key concepts with commentary |

**Story mode keyboard shortcuts:** `←` `→` to navigate, `Esc` to exit.

## Concepts covered

The graph is organised into 15 clusters radiating from a central thesis (*tools we use are not completely subordinate to our will*):

- **Not neutral** — Heidegger's enframing, substantive vs. instrumental views, silent legislation
- **Device paradigm** — Borgmann on focal practices and commodious consumption
- **Pharmakon** — Stiegler on tertiary retention, affective atrophy, proletarianisation of the mind
- **Contingent** — Feenberg on primary/secondary instrumentalisation and democratic rationalisation
- **Inscription** — Latour on black-boxing, obligatory passage points, translation
- **Socially constructed** — Bijker & Pinch, rhetorical closure, civic epistemology, co-production
- **Hegemony** — Gramsci, Foucault on disciplinary power, governmentality, normalisation
- **Social imaginary** — Taylor, sociotechnical imaginaries, print capitalism, soft despotism
- **Agonism** — Mouffe on antagonism vs. agonism, consensus as erasure
- **Adversarial design** — DiSalvo on surfacing conflict, critical design, breaking enframing
- **Defuturing** — Fry on structural lock-in, ontological design, sustainment
- **Foreclosed futures** — actual vs. possible vs. past futures, hindsight determinism
- **Futuring** — Bendor's forecast/backcast/recast/pastcast methods, the Polak pull
- **Democratic imagination** — Bendor on participatory governance, Research through Design
- **Value Sensitive Design** — direct/indirect stakeholders, three investigations, value conflicts

## Technical notes

A single self-contained `index.html` — no build step, no dependencies beyond two Google Fonts. The graph is rendered as inline SVG with quadratic Bézier edges. Pan and zoom are handled via an SVG `transform` attribute updated on pointer and wheel events.

The file passes WCAG 2.1 AA: all text and UI components meet contrast thresholds, every interactive element is keyboard-focusable with visible focus indicators, and the story panel is fully navigable without a mouse.

## Running locally

```bash
open index.html        # macOS
start index.html       # Windows
xdg-open index.html    # Linux
```

Or serve it with any static file server:

```bash
npx serve .
python3 -m http.server
```
