0a. Study `progress_checklist.md` and `pages/*.html` with up to 500 parallel Sonnet subagents to learn the application specifications and current content style (Penguin Books, Double Density).
0b. Study @IMPLEMENTATION_PLAN.md.
0c. For reference, the application source code is in `src/*` (actually `pages/` and `style.css` in this root).

1. Your task is to implement functionality per the specifications using parallel subagents. Follow @IMPLEMENTATION_PLAN.md and choose the most important item to address.
    *   **If updating an existing page:** READ IT FIRST. Do not destroy existing good content. EXPAND it. Add tables, explanations, and drills.
    *   **If fixing UI:** Remove inline styles that look old (solid black borders, default table styles). Use existing `style.css` classes or create modern, sleek CSS variables. Aim for "Modern Penguin Book" aesthetic, not "Retro Software".

2. **Validation (Backpressure):**
    *   **Density Check:** Is the page scrollable? (It should be long). Does it have at least 3 distinct sections (Grammar, Vocab, Drill)?
    *   **UI Check:** Does it match the best pages in the project? (Compare with a known good page).
    *   **Language Check:** Is the narrative **Turkish**? Are linguistic terms **English**? Are examples **Feminine**?

3. After implementing functionality or resolving problems, validate the work. Ultrathink.
4. When you discover issues, immediately update @IMPLEMENTATION_PLAN.md with your findings using a subagent. When resolved, update and remove the item.
5. When the validation passes, update @IMPLEMENTATION_PLAN.md, then `git add -A` then `git commit` with a message describing the changes. After the commit, `git push`.

99999. Important: When authoring content, capture the cultural and linguistic nuance.
999999. Important: Single sources of truth. If links are broken, resolve them.
9999999. As soon as there are no errors create a git tag. If there are no git tags start at 0.0.0 and increment patch by 1.
99999999. You may add extra logging if required to debug issues.
999999999. Keep @IMPLEMENTATION_PLAN.md current with learnings using a subagent. Update especially after finishing your turn.
9999999999. When you learn something new about how to run the application, update @AGENTS.md using a subagent but keep it brief.
99999999999. For any bugs you notice, resolve them or document them in @IMPLEMENTATION_PLAN.md using a subagent.
999999999999. Implement functionality completely. No short pages.
9999999999999. When @IMPLEMENTATION_PLAN.md becomes large periodically clean out the items that are completed from the file using a subagent.
99999999999999. If you find inconsistencies in the content then use an Opus 4.5 subagent with 'ultrathink' requested to update the specs/pages.
999999999999999. IMPORTANT: Keep @AGENTS.md operational only.