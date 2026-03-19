# Palette's Journal

## 2025-05-14 - [Font-Loading and Fixed Dimensions]
**Learning:** Using fixed dimensions (like `width` and `height`) on elements that rely on icon fonts (like Material Icons) can cause severe visual regressions if the font fails to load or is delayed. The fallback text will often exceed the fixed dimensions and overlap with neighboring elements.
**Action:** Use `min-width` instead of `width` for icon buttons and provide sufficient padding. Always consider how the interface looks with fallback text.

## 2025-05-14 - [Inconsistent Component Initialization]
**Learning:** When adding a new feature that involves template-based creation (like `createSheet`), it's easy to forget to update the static initial state in the HTML.
**Action:** Always verify that functional changes are applied to both dynamically generated elements and the initial static DOM.

## 2025-05-15 - [Emoji vs. Icon Consistency]
**Learning:** Mixing emojis and icon fonts (like Material Icons) creates a disjointed UX. Material Icons provide a more professional, "tool-like" interface that aligns with MD3 standards and offers better accessibility through clear ligatures.
**Action:** Replace platform-dependent emojis with a consistent icon font for all tool-centric UI elements.
