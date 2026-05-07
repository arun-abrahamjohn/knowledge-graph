# Technology · Power · Futures

An interactive knowledge graph mapping key concepts in the philosophy of technology — from Heidegger's enframing to democratic imagination, adversarial design to foreclosed futures.

<img width="1405" height="794" alt="image" src="https://github.com/user-attachments/assets/831b92ff-e151-406f-9283-a04583330be0" />



## Using the graph

| Action | How |
|--------|-----|
| Start guided tour | Click **Guided tour** in the top bar |
| Navigate tour steps | Use `←` and `→`, or click the side arrows |
| Exit guided tour | Click **Exit tour** or press `Esc` |
| Inspect highlighted concepts | Hover highlighted nodes during the tour to see context tooltips |
| Search concepts | Type in the search box (top right) |
| Reset view and filters | Click **Reset** in the toolbar |

**Guided tour keyboard shortcuts:** `←` `→` to navigate, `Esc` to exit.

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

A single self-contained `index.html` — no build step, no framework, and only Google Fonts as an external dependency.

The graph now uses a 3D sphere distribution projected into SVG, with continuous Y-axis auto-rotation and depth-based opacity. During the guided tour, each step focuses a concept, highlights connected nodes and edges, and smoothly zooms the camera to frame that local neighborhood.

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
