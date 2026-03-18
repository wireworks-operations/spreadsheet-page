# Scribe's Journal 📘

## 2025-05-14 - [Zero-Dependency Constraint]

**Observation:** The project is designed as a zero-dependency static
application with two parallel entry points (`index.html` and
`src/pages/spreadsheet.html`).

**Learning:** Documentation must emphasize that no build tools or package
managers are required for basic use, making it exceptionally easy to set up.
However, the lack of automated tests means manual verification is the
current standard.

**Action:** Updated `README.md` and `QUICKSTART.md` to highlight the
"zero-dependency" nature and provided simple local serving options
(Python/Node) to accommodate different environments.

## 2025-05-14 - [State Management & Persistence]

**Observation:** `index.html` uses direct DOM manipulation while
`spreadsheet.html` uses a state object and IndexedDB.

**Learning:** This architectural difference is a key insight for developers
looking to scale the project.

**Action:** Created `BLUEPRINT.md` to explain these differences using an
ASCII diagram and detailed component descriptions.
