# IMPLEMENTATION PLAN: Rusca Calis Textbook

## PROJECT STATUS OVERVIEW

**Last Updated:** 2026-01-28
**Status:** PHASE 1-3 COMPLETE - All 75 pages densified, ready for Phase 4
**Total Pages (Main Repo):** 75 pages (25KB-83KB each)
**Playbook:** 19 pages (FROZEN - archived)
**Quality Standard:** "Penguin Books Modern UI" + Pratik Sokak Ruscasi

---

## GERCEK PROJE AMACI

**Ukrayna'da yasayan kadin icin pratik sokak Ruscasi:**

| Hedef | Aciklama |
|-------|----------|
| **Sokakta tanisma** | Kizlarla tanismak, ilk temas, numara almak |
| **Flort ve davet** | Iltifat etmek, ilgi cekmek, eve/otele davet |
| **Cinsel iletisim** | Acik acik cinsel konulari konusmak, sinir belirlemek, onay almak |
| **Iliski anlatimi** | Erkek arkadasi tanitmak, durumu aciklamak, durust olmak |
| **Hikaye anlatma** | Maceralar, tecrubeler, yasanmisliklar paylasmak |
| **Pratik cumleler** | Hemen kullanilabilir, ezberlenebilir kaliplar |

### Tipik Senaryo

```
1. Disarida yalniz tanisiyorsun (bar, kafe, sokak)
2. Kizla flort ediyorsun
3. Erkek arkadasindan bahsediyorsun - durumu acikliyorsun
4. Maceralarini, tecrubelerini anlatiyorsun
5. Eve davet edip tanistiriyorsun
```

**Bu bir akademik ders kitabi DEGIL.** Akademik dilbilgisi ikinci planda. Oncelik: sokakta hemen ise yarar Rusca.

---

## COMPLETED WORK SUMMARY

### Phase 1-3: Complete (2026-01-13 to 2026-01-28)

**All 75 main repo pages densified to 25KB-83KB each.** See git history for detailed changes.

| Phase | Description | Status |
|-------|-------------|--------|
| **Phase 1** | Retroactive Upgrades - Skeleton/Severe/Inadequate pages | COMPLETE |
| **Phase 2** | Playbook Integration - CSS merged to main repo | COMPLETE |
| **Phase 3** | Content Bridge - Pages 06-16 created | COMPLETE |
| **Borderline Polish** | All borderline pages verified 34KB+ | COMPLETE |

**Key Milestones:**
- 2026-01-13: Initial CSS framework (15.7KB) and index.html
- 2026-01-25: Playbook pages 02-05 densified, Pages 17-23 (NSFW Core) all GOLD STANDARD
- 2026-01-26: Pages 24-75 densified (all skeleton/severe pages), Pages 06-16 created
- 2026-01-28: Pages 01-03 densified, Page 16 masterclass created, CSS merged, borderline polish complete

**Final Size Distribution:**
- All 75 pages: 25KB - 83KB (minimum standard: 15KB)
- Average page size: ~45KB
- Largest pages: page_71 (82.8KB), page_75 (77.4KB), page_72 (63KB)

**Git Tags:** main repo v0.0.38, playbook v0.0.25

---

## PHASE 4: ADVANCED CONTENT (Future - Pages 76-368)

### Proposed Batch Structure:

| Batch | Pages | Focus Area |
|-------|-------|------------|
| 1 | 76-95 | Cases Deep Dive (Accusative, Genitive) |
| 2 | 96-115 | Verb Aspects (Perfective/Imperfective) |
| 3 | 116-135 | Motion Verbs (idti/khodit) |
| 4 | 136-155 | Advanced Flirting & Compliments |
| 5 | 156-175 | Nightlife Scenarios |
| 6 | 176-195 | Relationship Vocabulary |
| 7 | 196-215 | Advanced NSFW Content |
| 8 | 216-235 | Conflict & Resolution |
| 9 | 236-255 | Slang Deep Dive |
| 10 | 256-275 | Internet/Text Russian |
| 11 | 276-295 | Cultural Deep Dives |
| 12 | 296-315 | Advanced Grammar |
| 13 | 316-335 | Reading Comprehension |
| 14 | 336-355 | Speaking Practice |
| 15 | 356-368 | Reference & Appendices |

---

## QUALITY CHECKLIST (Per Page)

Before marking ANY page complete, verify:

### Content (All Required)
- [ ] File size >= 15KB
- [ ] Vocabulary table: 10-15 words minimum
- [ ] Grammar boxes: 3-5 with color variants (blue, green, purple, orange)
- [ ] Drill sections: 3-4 exercises
- [ ] Cultural note: 1 section minimum
- [ ] Summary box: Present at end
- [ ] Dialogue/Reading: Where applicable

### Design (All Required)
- [ ] ZERO inline styles
- [ ] ZERO page-specific `<style>` blocks
- [ ] All CSS classes exist in style.css
- [ ] `.book-container` wrapper
- [ ] `.penguin-header` with h1, subtitle, page number
- [ ] `<main>` tag wrapping content
- [ ] `.page-navigation` with prev/next
- [ ] Consistent heading hierarchy (h2 > h3 > h4)

### Language (All Required)
- [ ] Main explanations in **Turkish**
- [ ] Technical terms in **English** (Case names, grammatical terms)
- [ ] Russian examples: Cyrillic + transliteration + Turkish
- [ ] Feminine verb forms prioritized (-la, studentka)
- [ ] No pure-English section headers

---

## CSS CLASSES (Reference)

The following custom classes are available in style.css:

```css
/* Main content styling */
.section-header-dark { }       /* Dark section headers */
.section-header-dark.with-accent { }
.highlight-box-yellow { }      /* Yellow highlight boxes */
.highlight-box-orange { }      /* Orange highlight boxes */
.emphasis-text { }             /* Emphasized text */
.ru-text { }                   /* Russian text styling */

/* Slang and intensity */
.slang-label { }               /* Labels for slang/mat/casual */
.slang-label.vulgar { }
.slang-label.mat { }
.slang-label.casual { }
.intensity { }                 /* Intensity dots */

/* Special content */
.scenario-box { }              /* Roleplay scenarios */
.safety-box { }                /* Consent/safety warnings */
.vocab-table-dark { }          /* Dark vocabulary tables */
.power-indicator { }           /* Power dynamics */

/* Core components */
.answer { }                    /* Answer styling */
.grammar-box-orange { }        /* Orange grammar boxes */
.grammar-box-blue { }          /* Blue grammar boxes */
.grammar-box-green { }         /* Green grammar boxes */
.grammar-box-purple { }        /* Purple grammar boxes */
```

---

## APPENDIX: GOLD STANDARD EXAMPLE

**Reference File:** `ralph-playbook/files/pages/page_04.html` (27.7KB)

This page demonstrates:
- Proper semantic structure (`<main>`, `<section>`, `<nav>`)
- Multiple grammar boxes with color variants
- Comprehensive vocabulary tables
- 7+ drill sections with varying formats
- 2 cultural notes with deep context
- 2 dialogues (formal and informal)
- Proper phonetics boxes with IPA
- Summary box at end
- Zero inline styles
- Turkish explanations with English technical terms
- Feminine-focused examples throughout

---

## RECENT CHANGES LOG (Last 10 Entries)

| Date | Item | Description |
|------|------|-------------|
| 2026-01-28 | BORDERLINE POLISH | All borderline pages verified dense (34KB-64KB) |
| 2026-01-28 | style.css | Playbook CSS components merged (447 lines) |
| 2026-01-28 | page_16.html | Masterclass: Mid-Term Review (44.3KB) |
| 2026-01-28 | pages 17-23 | Page numbers fixed to "Sayfa X / 75" |
| 2026-01-26 | pages 46-75 | All skeleton pages densified (30-83KB each) |
| 2026-01-26 | pages 24-45 | All severe pages densified (25-58KB each) |
| 2026-01-26 | pages 06-16 | New content bridge pages created |
| 2026-01-25 | pages 17-23 | NSFW Core all GOLD STANDARD |
| 2026-01-25 | CSS additions | Standardized classes for main repo |
| 2026-01-25 | pages 02-05 | Playbook pages densified |

---

*Document Version: 65.0*
*Last Updated: 2026-01-28*
*Project Status: PHASE 1-3 COMPLETE - All 75 main repo pages densified (25KB-83KB each). Playbook FROZEN at 19 pages. Ready for Phase 4 expansion (pages 76+) when needed.*
