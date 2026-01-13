0a. Study `progress_checklist.md`, `style.css`, and a sampling of `pages/*.html` (especially early vs recent pages) with up to 250 parallel Sonnet subagents to benchmark the current quality.
0b. Study @IMPLEMENTATION_PLAN.md (if present).
0c. Study `index.html` and `style.css` to understand the intended "Penguin Books" modern design system.
0d. For reference, the application source code is in the root directory.

1. **RETROACTIVE AUDIT & PLANNING:** Your primary task is to scan ALL existing pages (Page 1 to 75+) and perform a Gap Analysis against two strict standards:
    *   **Content Standard ("Double Density"):** Is the page a real textbook chapter? Does it have Grammar Boxes, Vocabulary Tables, Drills, and Cultural Notes? Or is it just a sparse HTML transcript? If sparse -> Plan a "Densification" task.
    *   **Design Standard ("Modern Book UI"):** Does it look like a premium web-book or "Windows 3.1"? Check for inconsistent margins, ugly default borders, or lack of visual hierarchy. If ugly -> Plan a "UI Overhaul" task.
    *   **Language Standard ("Bilingual Code-Switching"):** Is the main explanation in **Turkish**? Are technical/linguistic terms in **English** (e.g., "Instrumental Case", "Palatalization")? Is the target audience addressed with **Feminine** forms (e.g., "Gittim", "Yaptım" context implied as female)? Check for pure English pages and mark them for translation.

2. **Sequential Planning:** After auditing existing pages, plan the next batch of new pages (76+) as usual.

3. Use an Opus subagent to analyze findings and REWRITE @IMPLEMENTATION_PLAN.md. The plan should be a prioritized bullet list:
    *   **Phase 1: Retroactive Upgrades** (Fixing Pages 1-XX that failed the audit).
    *   **Phase 2: New Content** (Implementing Pages 76+ with the correct standard from the start).

**CRITICAL CRITERIA:**
*   **No Short Pages:** Every page must feel like a full lesson.
*   **Modern UI:** Use `style.css` classes effectively. Avoid inline styles that look dated.
*   **Feminine Focus:** Ensure examples are fem-centric.

ULTIMATE GOAL: A consistent, 368-page high-quality textbook. The user explicitly stated some pages look like "Windows 3.1" - find them and kill them.
