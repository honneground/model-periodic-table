# Model Periodic Table

An interactive, single-file UI concept prototype that replaces a traditional AI model dropdown with a full 118-element periodic table selector.

**Live Demo:** [https://honneground.github.io/model-periodic-table/](https://honneground.github.io/model-periodic-table/)

## Highlights

- **Full 118-Element Layout** — Standard 18-group × 7-period grid plus detached Lanthanides (`57–71`) and Actinides (`89–103`) rows with interactive series highlighting.
- **Instant Search & Filtering** — Search in real time by element name, symbol, or atomic number (`Escape` clears the filter).
- **Hover Preview & Click-to-Pin Cards** — Hovering any element displays a lightweight preview card; clicking pins the card in place and expands controls without losing cursor flow.
- **Smart Edge & Row Collision Detection** — Popover cards clamp horizontally near left/right panel edges and flip downward on top rows (`1–2`) so they never obscure the prompt bar.
- **Per-Model Thinking Level Memory** — Each released model independently remembers its `Low` / `Medium` / `High` setting via a sliding segmented control, and surfaces non-`Low` levels inline on the prompt bar trigger.
- **Prompt Bar Actions & Mode Switching** — Left `+` menu with file upload, web drive source, submenu uploads, creative tools, and a `Labs` toggle; hover tooltips with working `Ctrl+Shift+M` / `Ctrl+Shift+D` shortcuts; `Chat` / `Task` mode switch updating the headline, placeholder, and suggested prompts.
- **Split-Screen & Mobile Adaptation** — Automatically sinks the prompt bar to the bottom on laptop split screens (`<= 980px`) with upward-opening popovers, grouped suggestions, and an ambient glow bloom.
- **Zero Build Step** — Self-contained in a single `index.html` using React 18 UMD and Babel Standalone.

## Released vs. Upcoming Models

| Atomic No. | Element | Role | Default Thinking Level | Mode | Status |
| :--- | :--- | :--- | :--- | :--- | :--- |
| `1 H` | Hydrogen | Everyday help | `Medium` | Chat & Task | Released |
| `6 C` | Carbon | Most complex work | `Low` | Chat & Task | Released |
| `8 O` | Oxygen | Fast everyday tasks | `Low` | Task | Released |
| `10 Ne` | Neon | Code and analysis | `Medium` | Task | Released |
| `18 Ar` | Argon | Code and analysis | `Low` | Chat & Task | Released |
| `36 Kr` | Krypton | Most complex work | `High` | Task | Released |
| `All other 112` | — | Previewable in grid & prompt trigger | — | — | Coming soon |

## Quick Start

No installation or bundler required — open `index.html` directly in any modern browser, or serve the directory locally:

```bash
python -m http.server 8000
```

## Disclaimer

This project is a standalone frontend UI/UX concept prototype built for interactive exploration and demonstration.
