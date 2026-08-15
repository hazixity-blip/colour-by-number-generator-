# Color-by-Number Generator

A client-side web application that transforms user-uploaded images into printable, grid-based color-by-number templates and reference guides.

## Features

- **Client-Side Image Processing** — Upload and convert images directly inside the browser using modern HTML5 Canvas technology without uploading data to external servers.
- **Customizable Grid & Palette** — Adjust template parameters dynamically:
  - **Grid Size:** Modify pixel tile sizes for higher detail or simpler designs.
  - **Color Count:** Reduce image colors using K-means clustering (between 4 and 16 distinct colors).
  - **Region & Line Controls:** Filter out tiny isolated areas and adjust grid line thickness.
- **Automatic Template & Legend Generation** — Renders two distinct canvas views:
  - **Numbered Template:** Outline grid containing number markers for coloring.
  - **Color Reference:** Full-color preview showing the expected final result.
  - **Color Guide:** Visual legend mapping numbers to their corresponding RGB swatch.
- **Export Options** — Download high-resolution PNG outputs individually (Template, Answer Key, Color Guide) or export all assets together.

## Project Structure

- `index.html` — All-in-one standalone file containing the HTML UI layout, embedded CSS styling, and the complete JavaScript `ColorByNumberGenerator` engine.

## Setup & Local Development

No build steps, frameworks, or external package installations are required.

Open `index.html` directly in any web browser, or serve it using Python's local server:

```bash
python -m http.server 8080
