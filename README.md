# Steel Frame Digital Model — Parametric Viewer

A browser-based, interactive 3D visualizer for a parametric steel-frame building, built to explore the structural design workflow described in Itagaki Corporation's Mechanical Engineer job posting (2D drawings → 3D model → detail drawings → material take-off).

**Live demo:** _add your deployed link here after hosting (e.g. Netlify/Render)_

## What it does

- Generates a 3D steel frame (columns, primary/secondary beams, diagonal bracing) from adjustable parameters: bay count, bay size, story count, story height
- Every member is individually clickable and shows its ID, steel section, length, and weight
- A live material take-off table recalculates automatically as the model changes, based on standard JIS steel section unit weights
- Grid axis labels (A, B, C… / 1, 2, 3…) for spatial reference, similar to structural drawing conventions

## What it is not

This is a visualization and quantity-estimation tool, not a structural analysis or BIM application. It does not perform load calculations, code compliance checks, or clash detection against real geometry, and it does not produce IFC or other BIM-standard data. It was built to demonstrate workflow understanding and front-end/3D programming ability, not as a substitute for CAD/BIM software such as AutoCAD or Tekla Structures.

## Tech stack

- Plain HTML/CSS/JavaScript — single self-contained file, no build step
- [Three.js](https://threejs.org/) (r128) for 3D rendering, loaded via CDN
- No backend, no database — all calculations run client-side in the browser

## Running it locally

Just open `steel_frame_viewer.html` in any modern browser. No installation or server required.

## Deploying

This is a static site — it can be deployed for free on Netlify, Render (Static Site), GitHub Pages, or Vercel by pointing the host at this repository.

## Author

Pasumarthi Balaji — B.Tech CSE, Jain University, Bengaluru
