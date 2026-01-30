# IMPLEMENTATION PLAN: Rusca Calis Textbook

---

## ⚠️ KRITIK UYARI - MUTLAKA OKU ⚠️

### BU HATA BIR DAHA YAPILMAYACAK

**2026-01-29 Olayi:** Onceki Claude session'lari bu dosyayi yanlis "duzeltmis" ve submodule icinde yanlis sayfalar olusturmus. Bu tamamen YANLIS.

### HARDCODED PATHLER - DEGISTIRME

```
MAIN REPO (GERCEK PROJE):
├── Path: c:/Users/Sturm/Downloads/ruscacalis/
├── Pages: c:/Users/Sturm/Downloads/ruscacalis/pages/
├── CSS: c:/Users/Sturm/Downloads/ruscacalis/style.css
├── Index: c:/Users/Sturm/Downloads/ruscacalis/index.html
└── Sayfa Sayisi: 78+ (page_01.html - page_78.html ve devami)

SUBMODULE (PLAYBOOK - FROZEN/ARSIV):
├── Path: c:/Users/Sturm/Downloads/ruscacalis/ralph-playbook/
├── Pages: c:/Users/Sturm/Downloads/ruscacalis/ralph-playbook/files/pages/
├── Sayfa Sayisi: 19 (page_01.html - page_19.html) - FROZEN
└── Bu klasore YENI SAYFA EKLENMEYECEK!
```

### KURALLAR

1. **YENI SAYFALAR SADECE MAIN REPO'YA EKLENIR:**
   - `c:/Users/Sturm/Downloads/ruscacalis/pages/page_XX.html`

2. **SUBMODULE'A DOKUNMA:**
   - `ralph-playbook/files/pages/` klasoru FROZEN
   - Sadece 19 sayfa var ve kalacak

3. **BU DOSYAYI "DUZELTME":**
   - Bu dosyadaki bilgiler DOGRU
   - "Discrepancy" yok - main repo'da 78+ sayfa var
   - Submodule'da 19 sayfa var - bu DOGRU

4. **VERIFICATION:**
   - Yeni sayfa eklemeden once: `ls c:/Users/Sturm/Downloads/ruscacalis/pages/ | wc -l`
   - Submodule kontrolu: `ls c:/Users/Sturm/Downloads/ruscacalis/ralph-playbook/files/pages/ | wc -l` (19 olmali)

---

## PROJECT STATUS OVERVIEW

**Last Updated:** 2026-01-29
**Status:** PHASE 4 IN PROGRESS - Batch 1 (Pages 76-95: Cases Deep Dive)
**Total Pages (Main Repo):** 79 pages complete + Phase 4 expansion in progress
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
- All 75 pages: 20KB - 83KB (minimum standard: 15KB)
- Average page size: ~40KB
- Smallest pages: page_22 (20KB), page_21 (21.5KB), page_17 (23.6KB)
- Largest pages: page_71 (82.8KB), page_75 (77.4KB), page_72 (63KB)
- Note: All pages meet quality standards with full content (vocab, grammar, drills, dialogues, cultural notes)

**Git Tags:** main repo v0.0.43, playbook v0.0.34

---

## PHASE 4: ADVANCED CONTENT (Pages 76-368)

### Current Batch: **BATCH 1 - Cases Deep Dive (Pages 76-95)**

**Focus:** Accusative & Genitive cases in practical contexts
**Target:** 20 pages, each 25KB+ with full content

### Batch 1 Progress Tracker:

| Page | Topic | Status | Size |
|------|-------|--------|------|
| 76 | Accusative Case Introduction | ✅ COMPLETE | 72KB |
| 77 | Accusative with Animate Nouns | ✅ COMPLETE | 62KB |
| 78 | Accusative in Flirting Contexts | ✅ COMPLETE | 66KB |
| 79 | Accusative Practice & Drills | ✅ COMPLETE | 74KB |
| 80 | Genitive Case Introduction | ⏳ PENDING | - |
| 81 | Genitive of Possession | ⏳ PENDING | - |
| 82 | Genitive with Negation | ⏳ PENDING | - |
| 83 | Genitive with Numbers | ⏳ PENDING | - |
| 84 | Genitive in Relationship Talk | ⏳ PENDING | - |
| 85 | Genitive Practice & Drills | ⏳ PENDING | - |
| 86 | Cases in Questions (Kogo? Chto?) | ⏳ PENDING | - |
| 87 | Cases with Prepositions | ⏳ PENDING | - |
| 88 | Mixed Cases Practice | ⏳ PENDING | - |
| 89 | Cases in Dialogue: Bar Scenario | ⏳ PENDING | - |
| 90 | Cases in Dialogue: Date Scenario | ⏳ PENDING | - |
| 91 | Case Errors to Avoid | ⏳ PENDING | - |
| 92 | Feminine Case Endings Focus | ⏳ PENDING | - |
| 93 | Cases in Compliments | ⏳ PENDING | - |
| 94 | Cases Review & Summary | ⏳ PENDING | - |
| 95 | Cases Final Test | ⏳ PENDING | - |

### Full Batch Structure:

| Batch | Pages | Focus Area | Status |
|-------|-------|------------|--------|
| **1** | **76-95** | **Cases Deep Dive (Accusative, Genitive)** | **🔄 IN PROGRESS** |
| 2 | 96-115 | Verb Aspects (Perfective/Imperfective) | ⏳ PENDING |
| 3 | 116-135 | Motion Verbs (idti/khodit) | ⏳ PENDING |
| 4 | 136-155 | Advanced Flirting & Compliments | ⏳ PENDING |
| 5 | 156-175 | Nightlife Scenarios | ⏳ PENDING |
| 6 | 176-195 | Relationship Vocabulary | ⏳ PENDING |
| 7 | 196-215 | Advanced NSFW Content | ⏳ PENDING |
| 8 | 216-235 | Conflict & Resolution | ⏳ PENDING |
| 9 | 236-255 | Slang Deep Dive | ⏳ PENDING |
| 10 | 256-275 | Internet/Text Russian | ⏳ PENDING |
| 11 | 276-295 | Cultural Deep Dives | ⏳ PENDING |
| 12 | 296-315 | Advanced Grammar | ⏳ PENDING |
| 13 | 316-335 | Reading Comprehension | ⏳ PENDING |
| 14 | 336-355 | Speaking Practice | ⏳ PENDING |
| 15 | 356-368 | Reference & Appendices | ⏳ PENDING |

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
| 2026-01-30 | page_79.html | Accusative Practice & Drills (74KB) - kapsamli pratik |
| 2026-01-29 | page_78.html | Accusative in Flirting Contexts (66KB) - flort baglaminda |
| 2026-01-29 | page_77.html | Accusative with Animate Nouns (62KB) - canli isimler |
| 2026-01-29 | page_76.html | Accusative Case Introduction (72KB) - Phase 4 first page |
| 2026-01-29 | PHASE 4 START | Phase 4 begins - Batch 1 (Pages 76-95: Cases Deep Dive) |
| 2026-01-28 | PLAYBOOK AUDIT | Verified clean state: no inline styles, correct navigation |
| 2026-01-28 | BORDERLINE POLISH | All borderline pages verified dense (34KB-64KB) |
| 2026-01-28 | style.css | Playbook CSS components merged (447 lines) |
| 2026-01-28 | page_16.html | Masterclass: Mid-Term Review (44.3KB) |
| 2026-01-28 | pages 17-23 | Page numbers fixed to "Sayfa X / 75" |
| 2026-01-26 | pages 46-75 | All skeleton pages densified (30-83KB each) |
| 2026-01-26 | pages 24-45 | All severe pages densified (25-58KB each) |
| 2026-01-26 | pages 06-16 | New content bridge pages created |
| 2026-01-25 | pages 17-23 | NSFW Core all GOLD STANDARD |

---

## DATA INTEGRITY NOTE

**2026-01-30 FIX:** Submodule `eed4da971bad71ecd65de9a7bc9c079afff4cfb2` commit'ine reset edildi. Onceki yanlis commitler (8432af3 ve sonrasi) discard edildi. Bu commitlerde Claude yanlislikla main repo'yu gormezden gelip submodule icinde 41 sayfa olusturmustu. Bu tamamen YANLIS'ti.

**Dogru Durum:**
- Main repo: 78 sayfa (page_01 - page_78) + Phase 4 devam ediyor
- Submodule: 19 sayfa (FROZEN)

---

*Document Version: 73.0*
*Last Updated: 2026-01-30*
*Project Status: PHASE 4 IN PROGRESS - Batch 1 (Pages 76-95: Cases Deep Dive). 79 pages complete. Playbook FROZEN at 19 pages.*
*KRITIK: Submodule commit eed4da9'da FROZEN. Yeni sayfalar SADECE main repo'ya eklenir.*
