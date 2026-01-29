# IMPLEMENTATION PLAN: Rusca Calis Textbook

## PROJECT STATUS OVERVIEW

**Last Updated:** 2026-01-29
**Status:** PHASE 2 IN PROGRESS - Continuing Content Development
**Total Pages:** 24 pages complete + expansion in progress
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

### Phase 1: Foundation (Complete)

**19 pages complete, all meeting quality standards (20KB-52KB each)**

| Page | Topic | Size | Status |
|------|-------|------|--------|
| 01 | Introduction to Russian | 20KB | COMPLETE |
| 02 | Basic Greetings | 36KB | COMPLETE |
| 03 | Numbers and Time | 36KB | COMPLETE |
| 04 | Pronouns and Basics | 28KB | COMPLETE |
| 05 | Common Phrases | 40KB | COMPLETE |
| 06 | Verbs Introduction | 36KB | COMPLETE |
| 07 | Present Tense | 36KB | COMPLETE |
| 08 | Past Tense | 40KB | COMPLETE |
| 09 | Future Tense | 36KB | COMPLETE |
| 10 | Questions | 40KB | COMPLETE |
| 11 | Negation | 36KB | COMPLETE |
| 12 | Adjectives | 36KB | COMPLETE |
| 13 | Adverbs | 44KB | COMPLETE |
| 14 | Prepositions | 44KB | COMPLETE |
| 15 | Advanced Verbs | 48KB | COMPLETE |
| 16 | Mid-Term Review | 52KB | COMPLETE |
| 17 | NSFW Introduction | 32KB | COMPLETE |
| 18 | BDSM and Control | 36KB | COMPLETE |
| 19 | Oral and Social Media | 36KB | COMPLETE |

---

## PHASE 2: CASES AND GRAMMAR EXPANSION (Pages 20-40)

### Current Focus: Cases Deep Dive

**Target:** Create grammatically rich content focusing on Russian cases in practical contexts

### Progress Tracker:

| Page | Topic | Status | Size |
|------|-------|--------|------|
| 20 | Accusative Case Introduction | ✅ COMPLETE | 32KB |
| 21 | Accusative with Animate Nouns | ✅ COMPLETE | 41KB |
| 22 | Accusative in Flirting Contexts | ✅ COMPLETE | 38KB |
| 23 | Accusative Practice & Drills | ✅ COMPLETE | 40KB |
| 24 | Genitive Case Introduction | ✅ COMPLETE | 32KB |
| 25 | Genitive of Possession | ⏳ PENDING | - |
| 26 | Genitive with Negation | ⏳ PENDING | - |
| 27 | Genitive with Numbers | ⏳ PENDING | - |
| 28 | Genitive in Relationship Talk | ⏳ PENDING | - |
| 29 | Genitive Practice & Drills | ⏳ PENDING | - |
| 30 | Dative Case Introduction | ⏳ PENDING | - |
| 31 | Dative for Recipients | ⏳ PENDING | - |
| 32 | Instrumental Case Introduction | ⏳ PENDING | - |
| 33 | Prepositional Case Introduction | ⏳ PENDING | - |
| 34 | Cases with Prepositions | ⏳ PENDING | - |
| 35 | Mixed Cases Practice | ⏳ PENDING | - |
| 36 | Cases in Dialogue: Bar Scenario | ⏳ PENDING | - |
| 37 | Cases in Dialogue: Date Scenario | ⏳ PENDING | - |
| 38 | Case Errors to Avoid | ⏳ PENDING | - |
| 39 | Cases Review & Summary | ⏳ PENDING | - |
| 40 | Cases Final Test | ⏳ PENDING | - |

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

**Reference File:** `pages/page_04.html` (28KB)

This page demonstrates:
- Proper semantic structure (`<main>`, `<section>`, `<nav>`)
- Multiple grammar boxes with color variants
- Comprehensive vocabulary tables
- 7+ drill sections with varying formats
- Cultural notes with deep context
- Dialogues (formal and informal)
- Proper phonetics boxes with IPA
- Summary box at end
- Zero inline styles
- Turkish explanations with English technical terms
- Feminine-focused examples throughout

---

## RECENT CHANGES LOG (Last 10 Entries)

| Date | Item | Description |
|------|------|-------------|
| 2026-01-29 | v0.0.39 | Git tag for page_24 (Genitive Case Introduction) |
| 2026-01-29 | page_24.html | Genitive Case Introduction (32KB) - comprehensive intro, prepositions, "У меня есть" structure |
| 2026-01-29 | v0.0.38 | Git tag for page_23 (Accusative Practice & Drills) |
| 2026-01-29 | page_23.html | Accusative Practice & Drills (40KB) - comprehensive exercises, 19 drill sections |
| 2026-01-29 | v0.0.37 | Git tag for page_22 (Accusative in Flirting Contexts) |
| 2026-01-29 | page_22.html | Accusative in Flirting Contexts (38KB) - comprehensive flort vocabulary, dialogues, drills |
| 2026-01-29 | v0.0.36 | Git tag for page_21 (Accusative with Animate Nouns) |
| 2026-01-29 | page_21.html | Accusative with Animate Nouns (41KB) - comprehensive canlilik coverage |
| 2026-01-29 | v0.0.35 | Git tag for page_20 + IMPLEMENTATION_PLAN fix |
| 2026-01-29 | page_20.html | Accusative Case Introduction (32KB) - Phase 2 first page |
| 2026-01-29 | PLAN CORRECTED | Fixed discrepancy - actual page count is 19, not 78 |
| 2026-01-29 | AUDIT | Discovered IMPLEMENTATION_PLAN was out of sync with actual files |
| 2026-01-28 | page_19.html | Oral and Social Media (36KB) - final page of Phase 1 |
| 2026-01-28 | style.css | CSS components finalized (22KB) |
| 2026-01-28 | page_16.html | Masterclass: Mid-Term Review (52KB) |
| 2026-01-27 | pages 17-19 | NSFW content pages created |
| 2026-01-26 | pages 06-16 | Grammar foundations created |
| 2026-01-25 | pages 01-05 | Initial content pages |
| 2026-01-13 | Initial setup | CSS framework and index.html |

---

## DATA INTEGRITY NOTE

**2026-01-29:** Previous sessions incorrectly updated this plan file without creating actual HTML files. The plan claimed 78 pages and Phase 4 progress, but only 19 pages existed. This has been corrected. Always verify file existence before updating progress.

---

*Document Version: 76.0*
*Last Updated: 2026-01-29*
*Project Status: PHASE 2 IN PROGRESS. 24 pages complete. Genitive Case series started.*

