# SVG Vector Studio — SVG Editor & Artboard Tool

A zero-build, standalone HTML application (`index.html`) for importing and editing existing SVG files, resizing shapes/lines/text directly on the canvas, wrapping multi-line text, cropping the artboard, applying publication colour palettes, and exporting as high-DPI PNG, publication PDF, or clean SVG.

## Features
- **On-Canvas Bounding-Box Resizing:** Drag any of the 8 bounding-box handles on shapes, lines, callouts, and groups to resize directly on the canvas (plus endpoint handles `P1`/`P2` for `<line>` elements).
- **Text Size Drag-Scaling & Wrapping:** Drag corner handles on any `<text>` bounding box to scale `font-size`, or drag the cyan left/right pill handles (`W`/`E`) to wrap text into multi-line `<tspan>` rows (also controllable via Inspector width & line-height inputs or manual line breaks).
- **Artboard Resize & Crop (`Shortcut: C`):** Interactive on-canvas crop handles, Fit to Content, and exact viewBox/dimension presets.
- **Marquee Multi-Selection:** Left-click and drag on empty canvas or background rects to select, move, or resize multiple elements together.
- **Text Colour & Typography Inspector:** Dedicated text colour picker, hex input, and quick swatches that cleanly override inline CSS `style="fill:..."` and nested `<tspan>` fills.
- **Light / Dark Theme Toggle:** Switch between Light Mode and Dark Mode in the top bar (persisted in `localStorage`).
- **Publication Palettes & Export:** Remap chart series colours in one click and export as **PNG (up to 4x 300DPI)**, **PDF (Exact Artboard, A4, or US Letter)**, or **clean `.svg`**.
