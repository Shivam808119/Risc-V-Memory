# RISC-V Memory Deep Dive — plain static website

A multi-page, beginner-friendly guide focused on memory systems in SERV, PicoRV32, Ibex, VEGA, CV32E40P, Rocket Core, SweRV EH1, VexRiscv, SonicBOOM/BOOM and Shakti.

## Contents
- `index.html`: learning path and overview
- `lessons/`: 12 detailed concept lessons, from core basics to RTL investigation
- `cores/index.html`: comparison worksheet
- `cores/*.html`: one profile per core
- `assets/site.css`: shared styling
- `assets/site.js`: tiny navigation filter only
- `SOURCES-AND-SCOPE.md`: official source links and technical cautions

## Preview locally
Open `index.html` in a browser. No build tool, server, framework or package install is required. Keep the folder structure unchanged so links and styling continue to work.

## Publish with GitHub Pages
1. Extract the ZIP.
2. Create a GitHub repository, e.g. `riscv-memory-deep-dive`.
3. Upload the *contents* of this folder to the repository root (not the ZIP and not a nested folder wrapper).
4. Open repository **Settings → Pages**.
5. Select **Deploy from a branch**, branch `main`, folder `/(root)`, then Save.
6. After deployment, the site URL usually looks like `https://YOUR-USERNAME.github.io/riscv-memory-deep-dive/`.

## Study recommendation
Read the core overview first, then lessons 2–12 in order. After each lesson, open a core profile and verify the feature in the exact manual, RTL and configuration. Start with PicoRV32 for a small visible handshake, then compare Ibex/CV32E40P, then Rocket/VexRiscv, then BOOM.
