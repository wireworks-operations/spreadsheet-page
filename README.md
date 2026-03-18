# Interactive Excel Material Design 📘

<p align="left">
  <img src="https://img.shields.io/badge/License-MIT-blue.svg" alt="License MIT">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white"
    alt="HTML5 Badge">
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white"
    alt="CSS3 Badge">
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black"
    alt="JavaScript Badge">
  <img src="https://img.shields.io/badge/Material--Design-3-blue?style=flat&logo=material-design&logoColor=white"
    alt="Material Design 3 Badge">
</p>

An interactive, zero-dependency spreadsheet tool styled with
**Material Design 3**. Create, edit, and export your data directly from your
browser.

---

## 🚀 Getting Started

> **Verified:** This project is static and runs in any modern web browser.

### Prerequisites

- A modern web browser (Chrome, Firefox, Safari, or Edge)

### Setup & Run

1. **Clone the repository:**

   ```bash
   git clone https://github.com/scribe/interactive-excel-material-design.git
   cd interactive-excel-material-design
   ```

2. **Open the application:**
   - **Method 1:** Open `index.html` directly in your browser.
   - **Method 2:** Serve it locally using a simple server:

     ```bash
     # Python
     python3 -m http.server 8000
     # Node
     npx serve .
     ```

     Then, visit: `http://localhost:8000`

---

## ✨ Features

- **MD3 UI:** Pillbox buttons, icon-only toolbar, and responsive layouts.
- **Dark Mode:** Support for dark and light themes with a single toggle.
- **Dynamic Table Actions:** Add/delete rows and columns, merge cells, and
  manage multiple sheets.
- **Advanced Mockup:** A more robust version at `src/pages/spreadsheet.html`
  featuring:
  - **Undo/Redo:** Full support for cell edits and resizing.
  - **IndexedDB Persistence:** Automatically saves your work in your browser.
  - **Column/Row Resizing:** Drag-and-drop resizing for a custom view.
  - **Markdown Export:** Export your spreadsheet as a structured Markdown file.

---

## 🏗️ Architecture

See [BLUEPRINT.md](BLUEPRINT.md) for a detailed look at the system architecture
and design decisions.

<details>
<summary><b>Click to expand: High-level overview</b></summary>

The project is built using a **single-file-centric approach** for the main
application (`index.html`) to ensure zero dependencies and extreme portability.
The advanced mockup (`spreadsheet.html`) demonstrates a more sophisticated
state-management approach while still adhering to the zero-dependency principle.

- **Frontend:** HTML5, CSS3, Vanilla JS.
- **Persistence:** Local Storage / IndexedDB (for advanced version).
- **Styling:** Material Design 3 tokens and guidelines.

</details>

---

## 🧪 Testing

This project currently relies on manual testing for its UI and functionality.

<details>
<summary><b>Click to expand: Verification Checklist</b></summary>

- [x] **Core Functions:** Verify cell editing, adding/deleting rows, and
  merging.
- [x] **Theme Toggle:** Ensure light/dark mode transitions smoothly.
- [x] **Export:** Test both HTML and Markdown exports.
- [x] **Persistence:** Verify that data persists in IndexedDB for the advanced
  mockup.

</details>

---

## 🆘 Troubleshooting

- **Icons not loading:** Ensure you have an active internet connection to load
  Material Icons from Google Fonts.
- **IndexedDB errors:** Make sure your browser isn't in "Incognito" or
  "Private" mode, which might block local storage.
- **Layout issues:** If you notice overlapping icons, verify that your browser
  supports CSS Grid and Flexbox.

---

## 🧩 Contributing

Contributions are welcome! Please see [CONTRIBUTING.md](CONTRIBUTING.md) for
details on our code style and PR process.

---

## 🔒 Security

For reporting vulnerabilities and security guidelines, please see
[SECURITY.md](SECURITY.md).

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).
