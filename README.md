# ndimfractals
Pictures of 3d and 4d continued fractions fractals
# Inversion fractals

Interactive pictures of the invariant set of an iterated function system (IFS) built from inversions in spheres. It generalises continued fractions from the line to the plane, 3-space and 4-space.

For each lattice point `b` in ℕ×ℤ^(d−1), the map

    θ_b(x) = (x + b) / ‖x + b‖²

sends the open ball of radius ½ centred at (½, 0, …, 0) into itself. The images of the ball are disjoint balls that touch their neighbours. Iterating the maps draws the invariant set.

## Contents

| File | What it is |
|------|------------|
| `index.html` | The main page: background mathematics and a live 2D demo. |
| `3d.html` | The 3D set as a point cloud, with slice animations. Works on desktop, phone and WebXR headsets. |
| `4d.html` | A 3D slice of the 4D set whose cutting hyperplane rotates through four dimensions. Add `#hi` to the address for high quality (15M points). |

## Running it

These are static files, so there is nothing to install. Open `index.html` in a browser, or publish the folder with GitHub Pages or any static host.

- The viewers load three.js (version 0.147.0) from the jsDelivr CDN, so an internet connection is needed.
- For VR, the page must be served over `https`, which GitHub Pages does. Open it in a headset browser and press **Enter VR**.
- The high-quality 4D mode needs a few hundred MB of memory. Use it on a desktop or laptop, not a phone or standalone headset.

## What the pictures are

All pictures are random samples of the set, produced by a "chaos game": start at a point, repeatedly apply a randomly chosen map, and plot where the orbit lands.

- **Truncated alphabet.** The system has infinitely many maps. Each picture uses digits up to a bound, so the smallest pieces near the point 0 are missing or sparse.
- **Weighted sampling.** The weights only affect how dense regions look, not which points belong to the set.
- **Slices.** A slice is a thin slab of points, so it also includes a small neighbourhood on either side.

## Sign convention

With `x − b` instead of `x + b`, the same construction works in the mirror-image ball centred at (−½, 0, …, 0), and the pictures are reflected.

## Author and licence

Author: _Bas Lemmens_  
Licence: _MIT_
