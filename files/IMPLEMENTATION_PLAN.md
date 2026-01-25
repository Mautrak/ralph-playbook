# IMPLEMENTATION PLAN: Rusca Calis Textbook

## PROJECT STATUS OVERVIEW

**Last Updated:** 2026-01-25
**Total Target:** 368 pages
**Completed:** 5 pages (Pages 1-5)
**Quality Standard:** "Double Density" + "Penguin Books Modern UI"

---

## QUALITY AUDIT RESULTS

### Gap Analysis: Pages 1-5

| Page | Size | Content Score | Design Score | Language | Action Required |
|------|------|---------------|--------------|----------|-----------------|
| 01 | 19.7KB | **A+** (Full) | **A** | TR+EN | **GOLD STANDARD** - Use as template |
| 02 | 8.5KB | **B-** (43%) | **A** | TR+EN | **DENSIFY** - Add 10KB content |
| 03 | 8.9KB | **B-** (45%) | **A** | TR+EN | **DENSIFY** - Add 10KB content |
| 04 | 27.7KB | **A+** (Full) | **A** | TR+EN | **COMPLETE** - Densified 2026-01-25 |
| 05 | 8.1KB | **B-** (41%) | **A** | TR+EN | **DENSIFY** - Add 11KB content |

### Quality Benchmarks

**MINIMUM per page:**
- File size: 15KB+ (target 18-20KB for core lessons)
- Vocabulary table: 10-15 words
- Grammar boxes: 2-3 (using color variants: blue, green, purple, orange)
- Drill sections: 3-4 exercises
- Cultural note: 1 section
- Summary box: Required
- Dialogue/Reading: 1 section (where applicable)

**LANGUAGE STANDARD:**
- Main text: **Turkish** (Turkce)
- Technical terms: **English** (e.g., "Palatalization", "Nominative Case", "Vowel Reduction")
- Examples: **Cyrillic + Transliteration + Turkish translation**
- Persona: **Feminine** verb forms (e.g., "Geldim", "Yaptim", "-ла" endings prioritized)

**DESIGN STANDARD ("Penguin Books Modern UI"):**
- NO inline styles (zero tolerance)
- Use only `style.css` classes
- Required structure: `.book-container` > `.penguin-header` + `main` + `.page-navigation`
- Color-coded grammar boxes for visual hierarchy
- Clean typography with proper Cyrillic rendering

---

## PHASE 1: RETROACTIVE DENSIFICATION

**Priority: CRITICAL**
**Goal:** Bring Pages 2-5 to 15KB+ each

### Page 02 - Sesli Harfler (Vowels)
**Current:** 8.5KB | **Target:** 18KB

**Add:**
- [ ] Extended phonetics section with IPA chart for all 10 vowels
- [ ] "Iotified vowels" grammar box (Я, Е, Ё, Ю explanation)
- [ ] Dialogue: "Cafe scene" demonstrating vowel reduction in natural speech
- [ ] 2 additional drill sections (minimal pairs, vowel dictation)
- [ ] Feminine verb examples with vowel patterns (читала, писала, говорила)
- [ ] Audio pronunciation guide placeholder/notes
- [ ] Warning box for common Turkish speaker mistakes

### Page 03 - Sessiz Harfler (Consonants)
**Current:** 8.9KB | **Target:** 18KB

**Add:**
- [ ] Complete consonant cluster section (СТР, ЗДР, etc.)
- [ ] Assimilation rules grammar box (regressive voicing)
- [ ] Extended "False Friends" section with full comparison table
- [ ] Dialogue demonstrating consonant clusters in context
- [ ] 2 additional drills (tongue twisters, minimal pairs)
- [ ] Phonetics box with articulation diagrams/descriptions
- [ ] Cultural note expansion: regional consonant variations

### Page 04 - Selamlasmalar (Greetings) - COMPLETED
**Final:** 27.7KB | **Target:** 18KB | **STATUS: DONE**

**Added (2026-01-25):**
- [x] Summary box (required component)
- [x] Extended dialogue: Full "Meeting at a party" scenario (2 dialogues total)
- [x] Time-of-day greetings with clock examples (grammar-box-green)
- [x] Formal letter/email greeting conventions (grammar-box-blue)
- [x] Grammar box: Vocative case hints (grammar-box-orange)
- [x] Patronymic (отчество) explanation with examples (grammar-box-purple)
- [x] 8 drill sections (role-play, formal/informal sorting, patronymic creation)
- [x] 2 cultural notes (handshaking customs, cheek kissing, ты/вы transition)
- [x] Vocabulary table: 15 words
- [x] Phonetics box for "Zdravstvuyte" pronunciation
- [x] Warning box for social etiquette

### Page 05 - Kisisel Zamirler (Personal Pronouns)
**Current:** 8.1KB | **Target:** 18KB

**Add:**
- [ ] Accusative and Dative case forms preview table
- [ ] Reflexive pronoun себя introduction
- [ ] Extended dialogue with pronoun-heavy conversation
- [ ] Grammar box: Pronoun omission rules (pro-drop)
- [ ] Possessive pronouns preview (мой, твой, её)
- [ ] 2 additional drills (case transformation, pronoun substitution)
- [ ] Feminine-focused examples throughout
- [ ] Warning box: Common mistakes with ты/вы

---

## PHASE 2: NEW CONTENT CREATION (Pages 6-75)

**Standard:** All new pages must meet 15KB+ minimum from creation

### Batch 1: Pages 6-15 (Phonetics & Basic Grammar)
| Page | Topic | Key Components |
|------|-------|----------------|
| 06 | Vurgu ve Tonlama (Stress & Intonation) | Stress patterns, IK-1 through IK-5 intonation contours |
| 07 | Hece Yapisi (Syllable Structure) | Open/closed syllables, consonant clusters |
| 08 | Isimler - Giris (Nouns Introduction) | Gender system, animate/inanimate |
| 09 | Isim Cinsiyetleri (Noun Genders) | Masculine/Feminine/Neuter patterns |
| 10 | Yalinci Hal - Nominative Case | Subject function, -ы/-и plurals |
| 11 | Sifatlar - Giris (Adjectives) | Agreement rules, hard/soft stems |
| 12 | Olmak Fiili (To Be - Быть) | Present tense omission, past/future |
| 13 | Sahiplik (Possession) | У меня есть structure |
| 14 | Olumsuzluk (Negation) | Не, нет, никогда patterns |
| 15 | Sorular (Questions) | Question words, intonation |

### Batch 2: Pages 16-30 (Cases Introduction)
| Page | Topic |
|------|-------|
| 16-18 | Accusative Case (Belirtme Hali) - 3 pages |
| 19-21 | Genitive Case (Sahiplik Hali) - 3 pages |
| 22-24 | Dative Case (Yonelme Hali) - 3 pages |
| 25-27 | Instrumental Case (Vasita Hali) - 3 pages |
| 28-30 | Prepositional/Locative Case (Bulunma Hali) - 3 pages |

### Batch 3: Pages 31-45 (Verbs Foundation)
| Page | Topic |
|------|-------|
| 31-33 | Present Tense Conjugation (1st/2nd conjugation) |
| 34-36 | Past Tense (Gender agreement, -л/-ла/-ло/-ли) |
| 37-39 | Future Tense (Compound and perfective) |
| 40-42 | Aspect Introduction (Imperfective/Perfective) |
| 43-45 | Common Irregular Verbs (хотеть, мочь, есть) |

### Batch 4: Pages 46-60 (Expanding Vocabulary)
| Page | Topic |
|------|-------|
| 46-48 | Numbers 1-100 |
| 49-51 | Time Expressions |
| 52-54 | Family Members |
| 55-57 | Daily Routines |
| 58-60 | Food and Dining |

### Batch 5: Pages 61-75 (Intermediate Grammar)
| Page | Topic |
|------|-------|
| 61-63 | Adjective Declension (Full paradigm) |
| 64-66 | Comparative/Superlative |
| 67-69 | Adverbs |
| 70-72 | Prepositions with Cases |
| 73-75 | Review and Consolidation |

---

## PHASE 3: ADVANCED CONTENT (Pages 76-368)

### Batch Structure (20 pages each)

| Batch | Pages | Focus Topic |
|-------|-------|-------------|
| 1 | 76-95 | Cases consolidation and exceptions |
| 2 | 96-115 | Verb aspects deep dive |
| 3 | 116-135 | Motion verbs (идти/ходить system) |
| 4 | 136-155 | Verbal adjectives (participles) |
| 5 | 156-175 | Complex sentences |
| 6 | 176-195 | Conditional and subjunctive |
| 7 | 196-215 | Reported speech |
| 8 | 216-235 | Numbers, dates, time advanced |
| 9 | 236-255 | Prefixed verbs of motion |
| 10 | 256-275 | Participles deep dive |
| 11 | 276-295 | Gerunds and verbal nouns |
| 12 | 296-315 | Stylistics and register |
| 13 | 316-335 | Professional/academic Russian |
| 14 | 336-355 | Literary Russian |
| 15 | 356-368 | Reference materials and appendices |

---

## QUALITY ASSURANCE CHECKLIST

### Before marking ANY page complete:

**Content (must ALL be true):**
- [ ] File size >= 15KB (target 18-20KB)
- [ ] Vocabulary table: 10-15 words minimum
- [ ] Grammar boxes: 2-3 with color variants
- [ ] Drill sections: 3-4 exercises
- [ ] Cultural note: 1 section
- [ ] Summary box: Present
- [ ] Dialogue/Reading: Where applicable

**Design (must ALL be true):**
- [ ] ZERO inline styles
- [ ] All CSS classes exist in `style.css`
- [ ] `.book-container` wrapper used
- [ ] `.penguin-header` with title, subtitle, page number
- [ ] `.page-navigation` with prev/next links
- [ ] Consistent heading hierarchy (h2 > h3 > h4)

**Language (must ALL be true):**
- [ ] Main explanations in **Turkish**
- [ ] Technical terms in **English** (Nominative Case, Palatalization, etc.)
- [ ] Russian examples with Cyrillic + transliteration + Turkish translation
- [ ] Feminine verb forms prioritized (-ла endings, студентка, etc.)
- [ ] No pure-English pages

---

## CSS CLASSES REFERENCE

### Grammar Boxes (use for visual hierarchy)
- `.grammar-box` - Default (orange accent)
- `.grammar-box-blue` - Rules/patterns
- `.grammar-box-green` - Positive examples
- `.grammar-box-purple` - Special/advanced
- `.grammar-box-orange` - Warnings/exceptions

### Alert Boxes
- `.warning-box` - "Dikkat!" auto-prefix
- `.grammar-box-warning` - "Onemli Uyari!" auto-prefix
- `.tip-box` - "Ipucu" auto-prefix

### Content Sections
- `.cultural-note` - "Kulturel Not" auto-prefix
- `.drill-section` - "Aliştirma" badge auto-added
- `.summary-box` - Lesson recap
- `.phonetics-box` - IPA/pronunciation
- `.example-box` - Standalone examples
- `.dialogue` + `.dialogue-line` - Conversations

### Tables
- `.vocab-table` - Vocabulary (orange header)
- `.conjugation-table` - Verb/case paradigms (black header)

### Text Styling
- `.cyrillic` / `.russian` - Russian text
- `.transliteration` - Italic romanization
- `.translation` - Muted Turkish translation
- `.ipa` - IPA phonetic symbols

---

## PRIORITY EXECUTION ORDER

1. ~~**IMMEDIATE:** Densify Page 04 (lowest quality, missing summary)~~ **DONE 2026-01-25**
2. **HIGH:** Densify Pages 02, 03, 05
3. **STANDARD:** Create Pages 06-15 (next batch)
4. **ONGOING:** Continue sequential page creation

---

## COMPLETED

| Date | Item | Description |
|------|------|-------------|
| 2026-01-13 | style.css | Complete CSS framework (15.7KB) |
| 2026-01-13 | index.html | Cover page with navigation |
| 2026-01-13 | page_01.html | Cyrillic Alphabet - GOLD STANDARD (19.7KB) |
| 2026-01-14 | page_02.html | Vowels - Basic version (8.5KB) |
| 2026-01-14 | page_03.html | Consonants - Basic version (8.9KB) |
| 2026-01-14 | page_04.html | Greetings - Basic version (6.4KB) |
| 2026-01-14 | page_05.html | Pronouns - Basic version (8.1KB) |
| 2026-01-25 | page_04.html | **DENSIFIED** - Greetings & Introductions (27.7KB) |

---

*Document Version: 3.1*
*Last Updated: 2026-01-25*
*Project Status: PHASE 1 - RETROACTIVE DENSIFICATION IN PROGRESS (1/4 complete)*
