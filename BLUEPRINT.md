# Blueprint 🧱

> **Goal:** Provide a fast mental model—components, boundaries, and critical flows.

## System Overview

This project is a zero-dependency, static web application. It uses modern HTML5,
CSS3 (Material Design 3 principles), and vanilla JavaScript to provide an
interactive spreadsheet experience.

```text
                    +---------------------------+
                    |       User Browser        |
                    +-------------+-------------+
                                  |
                                  | Opens File
                                  v
                    +-------------+-------------+
                    |      Static Assets        |
                    | (HTML, CSS, Vanilla JS)   |
                    +-------------+-------------+
                                  |
             +--------------------+--------------------+
             |                                         |
             v                                         v
  +-----------------------+                 +-----------------------+
  |      Main App         |                 |   Advanced Mockup     |
  |    (index.html)       |                 | (spreadsheet.html)    |
  | Basic Editing, Export |                 | Undo/Redo, Resizing,  |
  | & Sheet Management    |                 | IndexedDB Persistence |
  +-----------------------+                 +-----------------------+
             |                                         |
             +--------------------+--------------------+
                                  |
                                  v
                    +---------------------------+
                    |    Browser Local Storage  |
                    |   (IndexedDB / LocalStor) |
                    +---------------------------+
```

## Data Flow (Happy Path)

1. **User interaction:** User clicks a cell or button in the UI.
2. **Event handling:** Vanilla JS event listeners capture the interaction.
3. **State update:**
   - In `index.html`, state is managed directly in the DOM and a few global
     variables.
   - In `spreadsheet.html`, a dedicated `state` object is updated and
     synchronized with the DOM.
4. **Persistence:**
   - `index.html` offers an HTML export option.
   - `spreadsheet.html` automatically saves to IndexedDB on command and
     maintains an Undo/Redo stack in memory.

## Key Files & Structure

- `index.html`: The primary entry point. A self-contained file containing all
  HTML, CSS, and JS for basic spreadsheet functionality.
- `src/pages/spreadsheet.html`: An advanced, more robust version of the
  spreadsheet with Material Design 3 tokens, Undo/Redo, and IndexedDB
  persistence.
- `CONTRIBUTING.md`: Guidelines for developers.
- `LICENSE`: MIT license details.

## Key Decisions

- **Zero Dependencies:** To ensure maximum portability and ease of setup, no
  external libraries or build tools (like React, Tailwind, or Webpack) are used.
- **Material Design 3:** The UI follows MD3 guidelines for a modern, accessible,
  and professional look.
- **Vanilla JS:** Leverages modern browser APIs for performance and simplicity.

## Risks & Trade-offs

- **Manual DOM Manipulation:** Without a framework like React, complex UI
  updates must be managed carefully to avoid performance issues or bugs.
- **Scalability:** As a client-side only app, data size is limited by browser
  storage constraints.
- **Consistency:** Maintaining feature parity between `index.html` and
  `spreadsheet.html` requires manual effort.
