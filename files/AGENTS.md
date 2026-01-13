## Build & Run

This is a static HTML/CSS project. There is no compile step.
To run: Open `index.html` or any `pages/page_XX.html` in a web browser.

## Validation

Run these checks after implementing a page:

- **Visual Check:** Ensure the page follows the "Penguin Books" Orange/Black/White theme. **AVOID "Windows 3.1" look:** No default HTML borders, no clunky buttons. Use sleek CSS.
- **Navigation:** Verify `<a href="page_PREV.html">` and `<a href="page_NEXT.html">` links are correct.
- **Content:** Ensure "Double Density" standard (Grammar boxes, Drills, Cultural Notes) is met. No empty or short pages.
- **Assets:** Ensure `../style.css` is correctly linked `<link rel="stylesheet" href="../style.css">`.

## Operational Notes

### Project Structure
- `index.html`: Cover page.
- `style.css`: Global styles (Penguin theme).
- `pages/`: Directory containing individual lesson pages (e.g., `page_01.html`).
- `progress_checklist.md`: Single source of truth for page conversion status.

### Critical Implementation Rules
1. **Double Density:** Every page must be rich. Explain "Why?" not just "What?". Add drills, nuances, and tables.
2. **Feminine Focus:** Examples should prioritize female speakers (using feminine past tense verbs like `poshla`, `sdelala`).
3. **Trilingual Flow (Code-Switching):**
    - **Base Narrative:** Turkish (Casual, conversational, engaging).
    - **Technical Terms:** English (e.g., "Past Tense", "Perfective Aspect").
    - **Content:** Russian (The material being taught).
4. **Phonetics:** Use 'IY' for 'Ы'.

### Codebase Patterns
- **HTML:** Modular files. pure HTML5 structure.
- **CSS:** `book-container`, `penguin-header`, `grammar-box`, `drill-section` classes are standard.
