# HADES Spectrometer — interactive 3D render

An in-browser, to-scale 3D model of the **HADES** forward spectrometer (GSI/FAIR),
built with [Three.js](https://threejs.org/). Open the live page:

**https://pjwinnetou.github.io/hades-spectrometer/**

Everything is in one self-contained file: [`index.html`](index.html) (HTML + CSS + JS).
Drag to orbit, scroll/pinch to zoom, toggle subsystems, use **Beam view** for the
head-on six-sector view.

## Geometry sources

Scene units are **metres**, beam along **+z**, target at the origin. Dimensions taken
from the public literature:

- **The HADES Collaboration**, *The high-acceptance dielectron spectrometer HADES*,
  **Eur. Phys. J. A 41, 243–277 (2009)** — [arXiv:0902.3478](https://arxiv.org/abs/0902.3478),
  [PDF at GSI](https://hades.gsi.de/sites/default/files/web/media/documents/EPJA2009.pdf).
- **The HADES Tracking System**, [arXiv:physics/0404011](https://arxiv.org/abs/physics/0404011).
- GSI HADES detector page — [hades.gsi.de/node/2](https://hades.gsi.de/node/2).

Values used: polar acceptance 18°–85°; 6 sectors with a 7° beam cone; START/VETO at
∓75 cm; RICH mirror radius 872 mm, mirror Ø 1440 mm, CaF₂ window Ø 1500 mm; MDC module
sizes 0.88×0.80 m (plane I) → 2.80×2.30 m (plane IV); 6 toroid coils (field between MDC
II and III), support ring Ø 3.56 m; TOF 44°–88°, TOFINO/RPC 18°–44°, META wall ≈2.1 m.

**Estimated:** the exact per-plane MDC z-positions (the HGeant geometry file is not
publicly accessible), derived here from module sizes and the acceptance angle.

## Disclaimer

Stylized model by Jaebeom & Claude from public references. **Not** official HADES
software or geometry, and not affiliated with the HADES Collaboration or GSI.
