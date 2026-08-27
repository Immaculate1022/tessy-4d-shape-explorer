# Meet Tessy! The 4D Shape Explorer

**A museum lab for curious brains · Tap, drag, and giggle with dimensions ✨**

Open-source interactive educational experience that introduces dimensions from **0D → 4D** and the tesseract (hypercube) in a playful, jargon-free way.

**Ages 8–12** · **No jargon** · **Works in any modern browser**

---

## Live Demo

Open [`index.html`](index.html) in any modern browser (or serve it statically).

No build step. No dependencies. Just pure HTML + Canvas + a little JavaScript.

---

## What kids (and grown-ups) learn

| Dimension | Character | Corners | Idea |
|-----------|-----------|---------|------|
| **0D** | Dotty | 1 | A single point |
| **1D** | Liney | 2 | A line (two ends) |
| **2D** | Squarey | 4 | A square on paper |
| **3D** | Cubey | 8 | A cube you can hold |
| **4D** | **Tessy** | **16** | A cube inside a cube + magic connections |

**Key insight** (shown live in the Corner Counter):  
Every time you add a new dimension you **double** the number of corners:

```
1 → 2 → 4 → 8 → 16
```

---

## Features

- Interactive **Story of Dimensions** cards (click Dotty → Tessy)
- Live **Canvas lab** – drag to spin the shape in 4D projection space
- Auto-spin mode
- Click vertices to highlight them
- Real-time **Corner Counter** that updates with the current dimension
- Touch-friendly (works on phones & tablets)
- Zero external libraries

---

## How the 4D projection works (for the curious)

Tessy is a **tesseract** (4-dimensional hypercube).  
We cannot see 4D directly, so the code:

1. Generates the 16 vertices of the unit tesseract (`±1, ±1, ±1, ±1`)
2. Applies rotations in the six 4D planes (XY, XZ, XW, YZ, YW, ZW)
3. Perspective-projects from 4D → 3D → 2D for the canvas

The result is the classic “cube inside a cube with connecting edges” visualization.

---

## Quick start

```bash
git clone https://github.com/Immaculate1022/tessy-4d-shape-explorer.git
cd tessy-4d-shape-explorer
# Just open index.html in a browser
# or serve it:
python -m http.server 8000
```

---

## Part of the PegaConstellation open-source collection

Related projects:

- [tesseract-medium](https://github.com/Immaculate1022/tesseract-medium) — advanced 4D non-orientable fractal geometry substrate
- [aetherius-nexus](https://github.com/Immaculate1022/aetherius-nexus) — interactive physics research platform
- [IOF-Resonance-Core](https://github.com/Immaculate1022/IOF-Resonance-Core) — high-dimensional resonance platform

---

## License

**IOF Attribution License v1.0** (or compatible open license)

Any public use or derivative work should include clear attribution to:

> PegaConstellation / Tessy 4D Shape Explorer by Gregory Scott Davis, Princeton, NC.

Educational remixing is encouraged!

---

## Credits

Inspired by dimensional storytelling and classic tesseract visualizations.  
Built to be simple, delightful, and fully open.
