# Palette's Journal

## 2025-05-14 - [Font-Loading and Fixed Dimensions]
**Learning:** Using fixed dimensions (like `width` and `height`) on elements that rely on icon fonts (like Material Icons) can cause severe visual regressions if the font fails to load or is delayed. The fallback text will often exceed the fixed dimensions and overlap with neighboring elements.
**Action:** Use `min-width` instead of `width` for icon buttons and provide sufficient padding. Always consider how the interface looks with fallback text.

## 2025-05-14 - [Inconsistent Component Initialization]
**Learning:** When adding a new feature that involves template-based creation (like `createSheet`), it's easy to forget to update the static initial state in the HTML.
**Action:** Always verify that functional changes are applied to both dynamically generated elements and the initial static DOM.
