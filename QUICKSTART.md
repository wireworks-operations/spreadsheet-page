# Quickstart ⚡

This path gets you from **clone → running app** with minimal steps.

## Prerequisites

- A modern web browser (Chrome, Firefox, Safari, or Edge)

## 1) Clone & enter

```bash
git clone https://github.com/scribe/interactive-excel-material-design.git
cd interactive-excel-material-design
```

## 2) Running the App

### Option A: Open directly (Simplest)

Just open `index.html` in your browser.

```bash
# Windows
start index.html
# macOS
open index.html
# Linux
xdg-open index.html
```

### Option B: Use a simple local server

If you want to use features like IndexedDB or just prefer a proper URL, run a
simple server:

```bash
# Python
python3 -m http.server 8000
# Node
npx serve .
```

Then, visit: `http://localhost:8000`

## 3) Try it out

1. **Add some data:** Click on any cell and start typing.
2. **Format it:** Use the toolbar (bottom-right toggle) to apply colors.
3. **Advanced Features:** Explore the more robust version at
   `src/pages/spreadsheet.html`.
4. **Save/Export:** Use the export button to download your work.

For deeper setup and architecture, see the [README](README.md) and
[BLUEPRINT](BLUEPRINT.md).
