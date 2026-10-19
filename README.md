# SVG Vector Studio — SVG Editor & Artboard Tool

A zero-build, standalone HTML application (`svg_editor.html`) designed for importing and editing existing SVG files, resizing or cropping the artboard, applying publication colour palettes, and exporting as high-DPI PNG, publication PDF, or clean SVG.

## Quick Start

1. Open [`svg_editor.html`](./svg_editor.html) (or [`src/index.html`](./src/index.html)) directly in any modern browser (Chrome, Safari, Edge, or Firefox).
2. Click **📂 Import SVG** (or drag and drop any `.svg` file onto the canvas), or click **</> SVG Code** to paste raw SVG XML.

## Key Features

### 1. Artboard Resize & Crop (` Crop / Artboard` Tool & `📐 Artboard` Tab)
- **Interactive On-Canvas Crop & Resize (`Shortcut: C`):** Drag any of the 8 handles around the artboard crop frame on the canvas (or drag inside the frame to reposition the crop region), then click **✓ Apply** (or press `Enter`).
- **Fit Artboard to Content (`⊡ Fit Artboard to Content`):** Automatically calculates the tight bounding box of all visible SVG elements with customizable padding (`px`) and crops/resizes the artboard around them.
- **Exact Numeric Dimensions & ViewBox Offset:** Set exact `X Offset`, `Y Offset`, `Width (px)`, and `Height (px)` in the `📐 Artboard` tab, with options to **Lock Aspect Ratio** or **Scale artwork proportionally with artboard**.
- **Quick Artboard Size Presets:** One-click presets for Inline Figure (`1200×580`), 16:9 Presentation (`1920×1080`), 16:9 Widescreen (`1600×900`), 4:3 Report (`1200×900`), 1:1 Square (`1080×1080`), A4 Landscape (`1123×794`), A4 Portrait (`794×1123`), and Compact Web (`800×600`).

### 2. Smart Publication Colour Palettes (`🎨 Palettes` Tab)
- **Bundled Palettes:**
  - **HKU SciFac — Muted Science:** `#4A6B6C`, `#C27D65`, `#D4B473`, `#6B8E73`, `#5C7487`, `#68627B`, `#A88B7D`
  - **HKU SciFac — Colour-Blind Safe (RYB):** `#1B4F72`, `#D1493E`, `#F2B705`, `#2B6CB0`, `#E05A47`, `#63B3ED`, `#9B2226`
  - **Journal & Editorial Standards:** *Nature Publishing Group (NPG)*, *Science / AAAS*, *The Lancet*, *Okabe-Ito Universal Accessible*, and *The Economist*.
- **Smart Series Remapping:** Clicking any palette automatically remaps detected accent/series colours across the SVG while preserving backgrounds (`#FFFFFF`, `#F8FAFC`, `#F1F5F9`) and structural text/grid neutrals (`#0F172A`, `#334155`, `#64748B`).
- **Auto-Contrast Text Guard:** Automatically switches label text sitting inside recoloured bars between `#FFFFFF` and `#222222` to maintain WCAG contrast.

### 3. Interactive Canvas, Marquee Multi-Selection & Alignment (`✏️ Inspector` Tab)
- **Marquee Multi-Selection:** Hold down the left mouse button and drag on any empty canvas area or background panel to draw a marquee selection box and select multiple elements at once (`Shift + Drag` to add to your existing selection).
- **Element vs. Group Dragging:** Click any shape or label to drag it (or drag any element in a multi-selection to move all selected elements together), or toggle **⧉ Drag Mode: Group (`<g>`)** (or hold `Alt` while clicking) to select and reposition entire `<g>` groups.
- **Smart Alignment & Snapping Guides:** Live magenta center and edge snap guides appear while dragging; use the 8-button Alignment & Distribution bar in the Inspector to align or distribute single or multi-selected (`Marquee Drag` or `Shift+Click`) elements.
- **Direct Text & Styling Controls:** Double-click any `<text>` element on the canvas for inline editing, or use the Inspector to adjust font family, size, weight, text anchor, letter spacing, fill/stroke colours, opacity, dash patterns, and corner radius.

### 4. Export as PNG, PDF & Clean SVG
- **🖼 Export as PNG:** Export crisp raster images at **1x**, **2x (Retina Slides)**, **3x (Print Report)**, or **4x (Ultra-HD 300DPI)** with original, pure white (`#FFFFFF`), or transparent alpha backgrounds.
- **📄 Export as PDF:** Export self-contained, high-resolution publication PDFs sized either to the **Exact Artboard Dimensions (1:1)** or fitted onto **A4 Landscape/Portrait** or **US Letter Landscape/Portrait** pages at **2x (150 DPI)**, **3x (300 DPI Print)**, or **4x (Ultra-HD Archival)** resolution.
- **⬇ Export SVG:** Download the clean, standards-compliant edited `.svg` file.
