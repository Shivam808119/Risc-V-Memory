# RISC-V Security Deep Dive

A static, multi-page HTML learning website for understanding hardware security and investigating ten RISC-V core families.

## Open locally
Open `index.html` in a modern browser. No server, framework, package manager or build step is required.

## Publish with GitHub Pages
1. Extract the ZIP.
2. Create a GitHub repository, e.g. `riscv-security-deep-dive`.
3. Upload the **contents** of this folder to the repository root (not the ZIP and not a nested folder).
4. Open **Settings → Pages**.
5. Choose **Deploy from a branch**, select `main` and `/(root)`, then save.
6. After deployment, the site will be available at `https://YOUR-USERNAME.github.io/riscv-security-deep-dive/`.

## Contents
- `index.html` — learning hub and study sequence
- `lessons/` — 12 detailed lessons on core concepts, privilege, PMP/Smepmp, virtual memory, secure boot, debug, side channels, integrity, crypto, DMA and verification
- `cores/` — overview and ten security profiles
- `glossary.html` — beginner-friendly definitions
- `assets/site.css` — styling
- `assets/site.js` — navigation search
- `SOURCES-AND-SCOPE.md` — references and caveats

## Important
This is a study guide, not a guarantee that any feature exists in any particular core. Confirm the exact RTL revision, configuration, firmware and SoC. The core profiles distinguish documented starting points from questions requiring verification.
