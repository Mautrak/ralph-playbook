# IMPLEMENTATION PLAN: Rusca Calis Textbook

## PROJECT STATUS OVERVIEW

**Last Updated:** 2026-01-26
**Status:** 🛑 PLAYBOOK FROZEN - Main Repo'ya odaklan
**Total Target:** 75 pages (main repo)
**Pages Existing (Main Repo):** 75 pages
**Pages Existing (Playbook):** 19 pages (page_01-19) - ARŞİVLENDİ
**Quality Standard:** "Penguin Books Modern UI" + Pratik Sokak Rusçası

---

## 🎯 GERÇEK PROJE AMACI

**Ukrayna'da yaşayan kadın için pratik sokak Rusçası:**

| Hedef | Açıklama |
|-------|----------|
| **Sokakta tanışma** | Kızlarla tanışmak, ilk temas, numara almak |
| **Flört ve davet** | İltifat etmek, ilgi çekmek, eve/otele davet |
| **Cinsel iletişim** | Açık açık cinsel konuları konuşmak, sınır belirlemek, onay almak |
| **İlişki anlatımı** | Erkek arkadaşı tanıtmak, durumu açıklamak, dürüst olmak |
| **Hikaye anlatma** | Maceralar, tecrübeler, yaşanmışlıklar paylaşmak |
| **Pratik cümleler** | Hemen kullanılabilir, ezberlenebilir kalıplar |

### Tipik Senaryo

```
1. Dışarıda yalnız tanışıyorsun (bar, kafe, sokak)
2. Kızla flört ediyorsun
3. Erkek arkadaşından bahsediyorsun - durumu açıklıyorsun
4. Maceralarını, tecrübelerini anlatıyorsun
5. Eve davet edip tanıştırıyorsun
```

**Bu bir akademik ders kitabı DEĞİL.** Akademik dilbilgisi ikinci planda. Öncelik: sokakta hemen işe yarar Rusça.

---

**Target Outcome:** Sokakta tanışma, flört, eve davet, cinsel konuşmalar

---

## ⚠️ DURUM DEĞİŞİKLİĞİ - 2026-01-26

**PLAYBOOK GENİŞLEMESİ DURDURULDU.**

Kullanıcı geri bildirimi: İki ayrı proje yerine TEK proje olmalı. Main repo'nun "sokak Rusçası" ruhu korunmalı. Playbook içeriği akademik ve yavaş - kullanıcının ihtiyacı hızlı, pratik, sokakta hemen kullanılabilir Rusça.

**YENİ STRATEJİ:**
1. Playbook'a yeni sayfa EKLEME
2. Playbook CSS'ini main repo'ya uygula
3. Playbook içeriğini main repo'ya opsiyonel bölümler olarak entegre et
4. Main repo sayfalarını (özellikle 10-25) düzelt ve güzelleştir
5. Main repo sayfalarini BITIR.
---

## EXECUTIVE SUMMARY

~~The project has **two parallel systems** that need to be **merged strategically**:~~

| Repository | Content Focus | Design Quality | Content Density | Pages | Durum |
|------------|--------------|----------------|-----------------|-------|-------|
| **Main Repo** | Street Russian (flirting, NSFW, nightlife) | 🔄 Güncelleniyor | 🔄 Artırılıyor | 75 | ✅ AKTİF |
| **Playbook** | Academic fundamentals (alphabet, grammar) | ✅ Modern Penguin | ✅ Dense (avg 30KB) | 19 | 🛑 FROZEN |

**THE NEW VISION:** Main repo TEK proje olarak kalacak. Playbook tasarım standartları main repo'ya uygulanacak. Playbook içeriği opsiyonel olarak gerektigi yerde main repoya ekstra icerik olarak appendlenecek ve bunun icin korunacak ama genişletilmeyecek.

---

## COMPREHENSIVE AUDIT RESULTS

### A. SIZE DISTRIBUTION (Main Repo - 75 Pages)

| Category | Size Range | Page Count | Pages | Priority |
|----------|-----------|------------|-------|----------|
| **SKELETON** | < 3KB | 23 | 46-56, 59-60, 62-63, 66-67, 69-75 | 🔴 CRITICAL |
| **SEVERE** | 3-4KB | 18 | 23-24, 30-34, 36, 38, 40-45 | 🔴 CRITICAL |
| **INADEQUATE** | 4-6KB | 22 | 06-11, 13-22, 25-29, 35 | 🟡 HIGH |
| **BORDERLINE** | 6-8KB | 7 | 01-05, 12, 58 | 🟡 MEDIUM |
| **ACCEPTABLE** | 8-15KB | 4 | 37, 39, 61, 64 | 🟢 POLISH |
| **GOOD** | 15KB+ | 1 | 65 (14.6KB) | 🟢 REVIEW |

**Summary:** 63 of 75 pages (84%) need major densification work.

### B. DESIGN FAILURES ("Windows 3.1" Syndrome)

Almost every page in the main repo contains:

```html
<!-- VIOLATION: Inline <style> blocks -->
<style>
    .kayf-box { border: 2px solid #ff9800; ... }
    .idiom-alert { border: 2px dashed #000; ... }
    .vulgar-header { background-color: #212121; color: #d32f2f; ... }
    .joke-break { border-left: 5px solid #FFC107; ... }
</style>

<!-- VIOLATION: Inline styles on elements -->
<div class="grammar-box" style="background-color:#ffebee;">
<p style="margin-top:10px;">
<div style="font-weight:bold; letter-spacing:1px; color:black;">
```

**Design Violations by Page:**

| Issue | Affected Pages | Fix Required |
|-------|---------------|--------------|
| Inline `<style>` block | ALL 75 pages | Remove, use style.css |
| Custom one-off classes | 60+ pages | Standardize or add to CSS |
| Old footer structure | ALL pages | Update to nav-based footer |
| Missing `<main>` tag | ALL pages | Add semantic structure |
| Missing `.penguin-header` subtitle | ALL pages | Add page context |
| Inconsistent heading hierarchy | 50+ pages | Standardize h2 > h3 > h4 |

### C. CONTENT FAILURES ("Empty Shell" Syndrome)

**Minimum Standard Per Page:**
- [ ] File size: 15KB minimum
- [ ] Vocabulary table: 10-15 words
- [ ] Grammar boxes: 3-5 (with color variants)
- [ ] Drill sections: 3-4 exercises
- [ ] Cultural note: 1 section
- [ ] Summary box: Required
- [ ] Dialogue/Reading: Where applicable

**Current Reality (Sample Audit):**

| Page | Size | Vocab Table | Grammar Boxes | Drills | Cultural Note | Summary | VERDICT |
|------|------|-------------|--------------|--------|---------------|---------|---------|
| 72 | 2.5KB | ❌ 0 | ❌ 1 | ❌ 1 | ❌ No | ❌ No | SKELETON |
| 46 | 2.7KB | ❌ 0 | ❌ 2 | ❌ 1 | ❌ No | ❌ No | SKELETON |
| 40 | 3.2KB | ❌ 0 | ❌ 1 | ❌ 1 | ❌ No | ❌ No | SKELETON |
| 17 | 24KB | ✅ 4 | ✅ 8 | ✅ 7 | ✅ 3 | ✅ Yes | **GOLD** |
| 65 | 14.6KB | ✅ 1 | ✅ 5 | ✅ 4 | ✅ Yes | ❌ No | BORDERLINE |
| PB-04 | 27.7KB | ✅ 3 | ✅ 8 | ✅ 7 | ✅ 2 | ✅ Yes | **GOLD** |

### D. LANGUAGE STANDARD COMPLIANCE

**Required Standard:**
- Main explanations: **Turkish** (Türkçe)
- Technical/linguistic terms: **English** (Nominative Case, Palatalization, Aspect)
- Russian examples: **Cyrillic + Transliteration + Turkish translation**
- Persona: **Feminine** verb forms prioritized (-ла endings, студентка)

**Violations Found:**

| Issue | Examples | Frequency |
|-------|----------|-----------|
| Pure English headers | "HIERARCHY OF FUCK", "Heavy Slang" | Common |
| Missing transliteration | Random across pages | Frequent |
| Missing Turkish translation | Some tables | Occasional |
| Masculine-defaulting | Most examples use он/он | Very Common |

---

## PHASE 1: RETROACTIVE UPGRADES (Priority)

### 1.1 CRITICAL SKELETON PAGES (23 pages, < 3KB)

**Pages:** 46, 47, 48, 49, 50, 51, 52, 53, 54, 55, 56, 59, 60, 62, 63, 66, 67, 69, 70, 71, 72, 73, 74, 75

**Action:** Complete rewrite. These pages are essentially empty placeholders.

**Template for Densification:**
1. Expand existing content to 3x-5x length
2. Add structured vocabulary table (10-15 words)
3. Add 3-5 grammar boxes with color coding
4. Add 3-4 drill sections
5. Add cultural note
6. Add summary box
7. Remove all inline styles
8. Add proper semantic structure

**Estimated Work:** ~4-6 hours per page

### 1.2 SEVERE UNDERDEVELOPMENT (18 pages, 3-4KB)

**Pages:** 23, 24, 30, 31, 32, 33, 34, 36, 38, 40, 41, 42, 43, 44, 45

**Action:** Major expansion. These have some content but are severely lacking.

### 1.3 INADEQUATE PAGES (22 pages, 4-6KB)

**Pages:** 06, 07, 08, 09, 10, 11, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 25, 26, 27, 28, 29, 35

**Action:** Moderate expansion + design fixes.

**Special Attention - NSFW CORE (Pages 17-23):**
These are the "destination" pages that the entire textbook leads to. They need EXTRA care:

| Page | Current | Topic | Priority |
|------|---------|-------|----------|
| 17 | 24KB | Heavy Slang & Negotiation | ✅ GOLD |
| 18 | ~22KB | BDSM / Control | ✅ GOLD |
| 19 | 26.8KB | Oral & Social Media | ✅ GOLD |
| 20 | 24.1KB | Negotiation & Finance | ✅ GOLD |
| 21 | 21.9KB | Conflict & Ultimatum | ✅ GOLD |
| 22 | 20.6KB | Body Map & Sensations | ✅ GOLD |
| 23 | 48.1KB | Roleplay & Scripts | ✅ GOLD |

### 1.4 BORDERLINE/ACCEPTABLE PAGES (11 pages, 6-15KB)

**Pages:** 01, 02, 03, 04, 05, 12, 37, 39, 58, 61, 64

**Action:** Design cleanup + minor content additions.

### 1.5 UNIVERSAL DESIGN FIX

Apply to ALL 75 pages:

1. **Remove inline styles** - Move to style.css
2. **Remove `<style>` blocks** - Standardize classes
3. **Add `<main>` semantic wrapper**
4. **Update header** to include subtitle and page number
5. **Update footer** to use `.page-navigation` structure
6. **Ensure heading hierarchy** (h2 > h3 > h4)
7. **Add missing CSS classes** to style.css

---

## PHASE 2: PLAYBOOK INTEGRATION

### 2.1 Playbook Page Densification

| Page | Current | Target | Topic | Status |
|------|---------|--------|-------|--------|
| 01 | 19.7KB | 20KB | Cyrillic Alphabet | ✅ GOLD |
| 02 | ~25KB | 18KB | Vowels | ✅ DENSIFIED |
| 03 | ~28KB | 18KB | Consonants | ✅ DENSIFIED |
| 04 | 27.7KB | - | Greetings | ✅ GOLD |
| 05 | ~30KB | 18KB | Pronouns | ✅ DENSIFIED |

### 2.2 Playbook Content Additions ✅ ALL COMPLETED

**Page 02 (Vowels) - DONE:**
- ✅ Extended phonetics section with IPA chart
- ✅ Iotified vowels grammar box (Я, Е, Ё, Ю)
- ✅ Dialogue: Cafe scene with vowel reduction
- ✅ 2 additional drill sections (8 total drills)
- ✅ Feminine verb examples (читала, писала)
- ✅ Warning box for Turkish speaker mistakes

**Page 03 (Consonants) - DONE:**
- ✅ Consonant cluster section (СТР, ЗДР)
- ✅ Assimilation rules grammar box
- ✅ Silent letters table
- ✅ Dialogue demonstrating clusters (airport scene)
- ✅ 9 drills (tongue twisters, minimal pairs included)

**Page 05 (Pronouns) - DONE:**
- ✅ Accusative/Dative preview table
- ✅ Reflexive pronoun себя introduction
- ✅ Extended pronoun dialogue (2 dialogues)
- ✅ Possessive pronouns preview
- ✅ 9 drills
- ✅ Warning box: ты/вы mistakes with consequences

---

## PHASE 3: CONTENT BRIDGE (New Pages 6-16)

These pages must bridge the academic foundation (Playbook 1-5) to the conversational content (Main Repo 10+).

### Proposed Curriculum (Academic → Practical):

| Page | Topic (Turkish) | Topic (English) | Key Grammar | Practical Application |
|------|-----------------|-----------------|-------------|----------------------|
| 06 | Vurgu ve Tonlama | Stress & Intonation | IK contours | Asking questions, expressing emotion |
| 07 | Temel Fiiller I | Basic Verbs I | хотеть, мочь | "I want", "Can you..." |
| 08 | Temel Fiiller II | Basic Verbs II | делать, идти | "What are you doing?", "Let's go" |
| 09 | Hal Sistemi - Giriş | Case System Intro | Overview | Understanding Russian word endings |
| 10 | Yalın Hal | Nominative Case | Subjects | "She is beautiful", "He is funny" |
| 11 | Sahiplik | Possession | У меня есть | "I have...", "Do you have..." |
| 12 | İstek ve Teklif | Wants & Offers | Давай, Хочешь | "Let's...", "Do you want to..." |
| 13 | Yer ve Yön | Location & Direction | Где/Куда | "Where is...", "Let's go to..." |
| 14 | Zaman İfadeleri | Time Expressions | сегодня, завтра | Making plans, scheduling |
| 15 | Sıfatlar | Adjectives | Agreement | Describing people, compliments |
| 16 | Karşılaştırma | Comparison | лучше, хуже | "Better", "Worse", preferences |

**Design Standard:** Each page must meet 15KB minimum with full component set.

---

## PHASE 4: ADVANCED CONTENT (Pages 76-368)

### Batch Structure (After Main Repo is Fixed):

| Batch | Pages | Focus Area |
|-------|-------|------------|
| 1 | 76-95 | Cases Deep Dive (Accusative, Genitive) |
| 2 | 96-115 | Verb Aspects (Perfective/Imperfective) |
| 3 | 116-135 | Motion Verbs (идти/ходить) |
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

## CSS CLASSES ADDED TO style.css ✅ COMPLETED

The following custom classes have been standardized and added:

```css
/* IMPLEMENTED 2026-01-25 */
.section-header-dark { }       /* ✅ Replaces .vulgar-header */
.section-header-dark.with-accent { }
.highlight-box-yellow { }      /* ✅ Replaces .joke-break */
.highlight-box-orange { }      /* ✅ Replaces .kayf-box */
.emphasis-text { }             /* ✅ Replaces .slang-word */
.ru-text { }                   /* ✅ Alias for .cyrillic */
.slang-label { }               /* ✅ NEW - labels for slang/mat/casual */
.slang-label.vulgar { }
.slang-label.mat { }
.slang-label.casual { }
.intensity { }                 /* ✅ NEW - intensity dots */
.scenario-box { }              /* ✅ NEW - roleplay scenarios */
.safety-box { }                /* ✅ NEW - consent/safety warnings */
.vocab-table-dark { }          /* ✅ Replaces .vulgar-table */
.power-indicator { }           /* ✅ NEW - power dynamics */

/* Already existed */
.answer { }                    /* ✅ Already in style.css */
.grammar-box-orange { }        /* ✅ Already in style.css (replaces .idiom-alert) */
```

---

## QUALITY CHECKLIST (Per Page)

Before marking ANY page complete, verify:

### Content (All Required)
- [ ] File size ≥ 15KB
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
- [ ] Feminine verb forms prioritized (-ла, студентка)
- [ ] No pure-English section headers

---

## PRIORITY EXECUTION ORDER

### Immediate (This Week)
1. [x] Densify Playbook pages 02, 03, 05 → 18KB each ✅ COMPLETED 2026-01-25
2. [x] Fix Pages 17-23 (NSFW Core) → 15KB+ each ✅ ALL 7 PAGES GOLD STANDARD 2026-01-25
3. [x] Create CSS additions for custom classes ✅ COMPLETED 2026-01-25

### High (Current Priority)
4. [x] Fix SKELETON pages (46-75) → 15KB each ✅ COMPLETED 2026-01-26 (30 pages densified)
5. [ ] Fix SEVERE pages (24-45) → 15KB each 🔴 IN PROGRESS (22 pages, currently 3-6KB each)

### Medium (After SEVERE)
6. [ ] Fix INADEQUATE pages (01-16) in main repo → 15KB each
7. [x] Create new Playbook pages 06-16 ✅ ALL COMPLETE (page_06 ✅, page_07 ✅, page_08 ✅, page_09 ✅, page_10 ✅, page_11 ✅, page_12 ✅, page_13 ✅, page_14 ✅, page_15 ✅, page_16 ✅)

### Ongoing (Month 2+)
8. [ ] Polish BORDERLINE pages (01-05, 37, 39, etc.)
9. [ ] Begin Phase 4 content (76+)

---

## COMPLETED

| Date | Item | Description |
|------|------|-------------|
| 2026-01-13 | style.css | Complete CSS framework (15.7KB) |
| 2026-01-13 | index.html | Cover page with navigation |
| 2026-01-13 | page_01.html | Playbook - Cyrillic Alphabet (19.7KB) |
| 2026-01-14 | page_02.html | Playbook - Vowels (8.5KB) |
| 2026-01-14 | page_03.html | Playbook - Consonants (8.9KB) |
| 2026-01-14 | page_04.html | Playbook - Basic version (6.4KB) |
| 2026-01-14 | page_05.html | Playbook - Pronouns (8.1KB) |
| 2026-01-25 | page_04.html | **DENSIFIED** - Greetings (27.7KB) ✅ GOLD STANDARD |
| 2026-01-25 | AUDIT | Comprehensive quality audit complete |
| 2026-01-25 | page_02.html | **DENSIFIED** - Vowels (~25KB) ✅ IPA charts, Iotated vowels, 2 dialogues, 8 drills |
| 2026-01-25 | page_03.html | **DENSIFIED** - Consonants (~28KB) ✅ Assimilation rules, clusters, tongue twisters, 9 drills |
| 2026-01-25 | page_05.html | **DENSIFIED** - Pronouns (~30KB) ✅ Case preview, себя, possessives, ты/вы warnings, 9 drills |
| 2026-01-25 | page_17.html | **DENSIFIED** - Argo & Pazarlik (24KB) ✅ Mat system, body slang, negotiation, rejection phrases, drug slang, 7 drills, 3 cultural notes |
| 2026-01-25 | page_18.html | **DENSIFIED** - BDSM & Kontrol (~22KB) ✅ Consent/safety vocab, imperative mood, positions, power dynamics, dirty talk, 2 dialogues, 6 drills, 2 cultural notes |
| 2026-01-25 | page_19.html | **DENSIFIED** - Oral & Social Media (26.8KB) ✅ Imperative mood, oral verbs, position directives, social media vocab, vape culture, 2 dialogues, 6 drills |
| 2026-01-25 | page_20.html | **DENSIFIED** - Negotiation & Finance (24.1KB) ✅ Money slang, price patterns, bargaining, payment methods, safety checks, 2 dialogues, 6 drills |
| 2026-01-25 | page_21.html | **DENSIFIED** - Conflict & Ultimatum (21.9KB) ✅ Conditional sentences, defense/offense phrases, de-escalation, Mat usage, 2 dialogues, 5 drills |
| 2026-01-25 | page_22.html | **DENSIFIED** - Body Map & Sensations (20.6KB) ✅ Detailed body parts, intimacy levels, sensory adjectives, touch verbs, reflexive себя, 2 dialogues, 5 drills |
| 2026-01-25 | page_23.html | **DENSIFIED** - Roleplay & Scripts (48.1KB) ✅ Power dynamics, role titles, command grammar, permission/denial, praise/punishment, safe words, aftercare, 3 scenarios, 2 dialogues, 6 drills |
| 2026-01-25 | style.css | **CSS ADDITIONS** - Standardized classes for main repo migration ✅ .section-header-dark, .highlight-box-yellow, .highlight-box-orange, .emphasis-text, .ru-text, .slang-label, .intensity, .scenario-box, .safety-box, .vocab-table-dark, .power-indicator |
| 2026-01-25 | page_06.html | **NEW** - Vurgu ve Tonlama (34.6KB) ✅ GOLD STANDARD - Stress patterns, vowel reduction, IK-1 to IK-5 intonation constructions, mobile stress in conjugation, 2 dialogues, 7 drills, 2 cultural notes |
| 2026-01-25 | page_07.html | **NEW** - Temel Fiiller I (36.8KB) ✅ GOLD STANDARD - хотеть (want) and мочь (can) conjugations, мочь vs уметь distinction, можно/нельзя, negation patterns, 2 dialogues, 6 drills, 2 cultural notes |
| 2026-01-25 | page_08.html | **NEW** - Temel Fiiller II (38.4KB) ✅ GOLD STANDARD - делать (to do/make) and идти/ходить (verbs of motion), unidirectional vs multidirectional distinction, давай/пойдём patterns, 2 dialogues, 6 drills, 2 cultural notes |
| 2026-01-25 | page_09.html | **NEW** - Hal Sistemi Giriş (36.2KB) ✅ GOLD STANDARD - Introduction to 6 Russian cases, Turkish-Russian case comparison, gender review, animacy distinction, 2 dialogues, 6 drills, 2 cultural notes |
| 2026-01-25 | page_10.html | **NEW** - Yalın Hal / Nominative Case (39.6KB) ✅ GOLD STANDARD - Adjective agreement, demonstrative pronouns, possessive pronouns, question formation, physical/personality adjectives, 2 dialogues, 7 drills, 2 cultural notes |
| 2026-01-25 | page_11.html | **NEW** - Sahiplik / Possession (34.2KB) ✅ GOLD STANDARD - У меня есть construction, genitive pronouns, negation with нет, есть omission rules, names in genitive, 2 dialogues, 7 drills, 2 cultural notes |
| 2026-01-25 | page_12.html | **NEW** - Istek ve Teklif / Wants & Offers (36.1KB) ✅ GOLD STANDARD - Давай/Давайте constructions, Хочешь patterns, accept/decline phrases, time/place specification, Мне хочется vs Я хочу, 2 dialogues, 7 drills, 2 cultural notes |
| 2026-01-26 | page_13.html | **NEW** - Yer ve Yon / Location & Direction (38.5KB) ✅ GOLD STANDARD - Где vs Куда distinction, Prepositional Case, Accusative with direction, В vs На prepositions, location adverbs, Откуда + Genitive, К + Dative for people, position verbs (стоять/лежать/сидеть/висеть), direction giving, 2 dialogues, 7 drills, 2 cultural notes |
| 2026-01-26 | page_14.html | **NEW** - Zaman Ifadeleri / Time Expressions (42.6KB) ✅ GOLD STANDARD - Basic time adverbs (сегодня/вчера/завтра), days of week with в+Acc and по+Dat, months with Prepositional, seasons with Instrumental, clock time, time prepositions (через/после/до/перед), day parts, frequency expressions, plan-making phrases, 2 dialogues, 7 drills, 2 cultural notes |
| 2026-01-26 | page_15.html | **NEW** - Sifatlar / Adjectives (49.9KB) ✅ GOLD STANDARD - Long vs short form adjectives, intensifiers (очень/слишком/довольно), color adjectives with синий vs голубой distinction, eye/hair color compounds, compliment patterns (Какая ты красивая!), advanced physical/personality adjectives, diplomatic negation, 2 dialogues, 7 drills, 2 cultural notes |
| 2026-01-26 | page_16.html | **NEW** - Karsilastirma / Comparison (50.3KB) ✅ GOLD STANDARD - Comparative formation (-ее/-ей), consonant mutations (к→ч, г→ж, х→ш, ст→щ), irregular comparatives (лучше/хуже/больше/меньше), superlative with самый, чем construction vs genitive, degree modifiers (гораздо/намного/немного), equality with такой же...как, preference expressions (больше нравится/предпочитаю), по- softening prefix, age comparison patterns, 2 dialogues, 7 drills, 2 cultural notes |
| 2026-01-26 | page_17.html | **NEW** - Argo ve Pazarlik / Slang & Negotiation (31.6KB) ✅ GOLD STANDARD - Mat system (4 root words), sexual activity verbs (politeness levels), body parts slang, negotiation phrases, rejection expressions (kibar→mat), drug slang, кайф etymology (from Turkish keyif!), reflexive verb conjugation, 2 dialogues, 8 drills, 3 cultural notes |
| 2026-01-26 | page_18.html | **NEW** - BDSM ve Kontrol / BDSM & Control (36.9KB) ✅ GOLD STANDARD - Consent vocabulary (согласие, границы, безопасное слово), traffic light system, power dynamics roles (дом/саб/Госпожа/Хозяин), Imperative mood formation, position commands (На колени!, Руки за спину!), comparative adverbs for intensity, praise/discipline phrases, BDSM equipment vocab, aftercare expressions, 2 dialogues, 8 drills, 2 cultural notes |
| 2026-01-26 | page_19.html | **NEW** - Oral ve Sosyal Medya / Oral & Social Media (34.8KB) ✅ GOLD STANDARD - Oral activity vocabulary (минет/куни, politeness levels), verb conjugations (сосать/лизать), consonant mutation (з→ж), sensory feedback expressions, Russian social media platforms (VK/Telegram/Odnoklassniki), messaging abbreviations (спс/пж/хз/кст), parenthesis smile culture )))/((( , flirt messaging patterns, emoji/sticker culture, 2 dialogues, 8 drills, 3 cultural notes |
| 2026-01-26 | All pages | **FIX** - Updated page numbers from "Sayfa X / 368" to "Sayfa X / 19" to reflect frozen playbook state ✅ |
| 2026-01-26 | index.html, style.css | **REFACTOR** - Moved cover page inline styles from index.html to style.css for consistency ✅ |
| 2026-01-26 | MAIN REPO page_46.html | **DENSIFIED** - Humor ve Sosyal Kalibrasyon (32.1KB) ✅ GOLD STANDARD - Komar joke, social validation phrases (Бинго!/Молодец!/Умница!), flirt signals (Типа, игра началась?), reflexive verb conjugation (смеяться/улыбаться), типа filler word usage, humor vocabulary table (12 words), 2 dialogues, 6 drills, 2 cultural notes, summary box |
| 2026-01-26 | MAIN REPO page_47.html | **DENSIFIED** - Pressure Tactics / Bahsi Arttirmak (37.2KB) ✅ GOLD STANDARD - За + Accusative time duration, urgency phrases (Сейчас или никогда/Время идёт/Это последний шанс), stakes raising (повышать ставки), Пока не construction, короче filler word, иначе conditional threats, повышать conjugation, 2 dialogues, 8 drills, 2 cultural notes, summary box |
| 2026-01-26 | MAIN REPO page_48.html | **DENSIFIED** - Zero Sum & Boundaries / Odesme ve Sinir Koyma (41.5KB) ✅ GOLD STANDARD - В ноль выходить construction (breaking even), boundary phrases (в пределах разумного, это мой предел, хватит vs достаточно), reflexive verbs (договориться, определиться) conjugation, reciprocity expressions (услуга за услугу, баш на баш - Turkce'den!), short-form adjectives (готов/согласен), выходить/выйти conjugation tables, 2 dialogues, 8 drills, 2 cultural notes, summary box |
| 2026-01-26 | MAIN REPO page_49.html | **DENSIFIED** - Trust Issues & Verification / Guvensizlik ve Dogrulama (44.7KB) ✅ GOLD STANDARD - Trust vocabulary (доверять/проверять/доказать), distrust expressions (Кто тебя знает/Откуда мне знать?), Пока не construction (until not), Imperative mood formation rules, physical commands (залезь/сядь/встань/ляг/подойди), skepticism phrases (Да ладно!/Врёшь!/Не верю), verification demands (Докажи/Покажи мне), "забрать и убежать" fear, Sovyet trust culture, 2 dialogues, 8 drills, 2 cultural notes, summary box |
| 2026-01-26 | MAIN REPO page_50.html | **DENSIFIED** - The Confrontation / Hesap Sorma ve Yakalanma (48.1KB) ✅ GOLD STANDARD - Confrontation questions (Что ты тут делаешь?/Что ты здесь забыла?), win/lose verbs (выиграть/проиграть) full conjugation, accusation patterns (Ты врала!/Тебя видели там!), defense expressions (Это не я!/Это не то что ты думаешь!), alibi vocabulary (свидетель/доказательство/алиби), phone tension phrases (Ну ответь да/Дай телефон!), признаться (confess) reflexive conjugation, otmazka (bahane) argo, Rus confrontation culture, 2 dialogues, 8 drills, 2 cultural notes, summary box |
| 2026-01-26 | MAIN REPO page_51.html | **DENSIFIED** - Phone Tension / Telefonda Gerilim ve Gizlilik (50.8KB) ✅ GOLD STANDARD - Phone/messaging vocabulary (сообщение/переписка/уведомление/пароль/блокировка), suspicion questions with Dative (Кому пишешь?) and Instrumental (С кем переписываешься?), phone imperatives (дай/покажи/положи/открой/разблокируй), privacy defense expressions (Это личное/Это не твоё дело/Ты мне не доверяешь?), delete/hide verbs (удалять/удалить, скрывать/скрыть) full conjugation, notification tension phrases, Чё/На slang usage, Russian relationship phone privacy culture, Telegram/VK messaging apps, 2 dialogues, 8 drills, 2 cultural notes, summary box |
| 2026-01-26 | MAIN REPO page_52.html | **DENSIFIED** - The Setup / Podstava: Kumpas, Tezgah ve Ihanet (51.6KB) ✅ GOLD STANDARD - Betrayal vocabulary (подстава/предательство/предать/сдать/слить/кинуть/кидала), "Что за...?" construction (saskinlik/ofke ifadesi), accusation questions (Ты что натворила?/Как ты могла?/Как ты посмела?), shaming expressions (Как тебе не стыдно?/У тебя совесть есть?/Где твоя совесть?), подставить vs предать distinction, сдать vs слить (polise vermek vs bilgi sizdirmak), кинуть para dolandiriciligi, defense/denial patterns (Я не виновата!/Это не я!/Это ложь!), counter-attack expressions (На себя посмотри!/Кто тебе это сказал?), Rus sadakat paranoyasi kulturel notu, "blin" ve diger yumusak kufur etimolojisi, 2 dialogues, 8 drills, 2 cultural notes, summary box |
| 2026-01-26 | MAIN REPO page_53.html | **DENSIFIED** - Breakup Pressure / Ayriliga Zorlama (53.7KB) ✅ GOLD STANDARD - Breakup vocabulary (расставание/расстаться/бросить/сложности/пора/тянуть), "Давай + verb" construction (Давай расстанемся/Давай не будем тянуть), "Пора + infinitive" construction (Пора расстаться/Тебе пора выбрать), расстаться/расставаться full conjugation (both aspects), бросить + Accusative (Брось её!/Он меня бросил), ultimatum patterns (Или я или она/Выбирай/Ты должен выбрать), excuse breaking (Какая разница?/Хватит отмазок!/Это просто отмазка), "вывести на чистую воду" idiom (ifsa etmek), "тянуть за нос" idiom (oyalamak), Rus ayrilik direkt kulturu, "otmazka" kulturu, 2 dialogues, 8 drills, 2 cultural notes, summary box |
| 2026-01-26 | MAIN REPO page_54.html | **DENSIFIED** - Moral Judgment / Ahlaki Yargilama ve Utandirma (49.0KB) ✅ GOLD STANDARD - Shame/judgment vocabulary (зашквар/позор/стыд/стыдно/мерзко/отвратительно), youth slang (кринж/треш/косяк), short-form adjectives (виноват/виновата, прав/права, готов/готова, достоин/достойна, способен/способна) with gender agreement, нельзя + infinitive prohibition pattern, reflexive shame verbs (позориться/стыдиться) full conjugation, dismissal imperatives (Уйди!/Отстань!/Отвали!/Пошёл вон!), classic shaming phrases (Как тебе не стыдно?/Стыд и позор!/Ты меня позоришь!), judgment patterns (Это предел!/Это последняя капля/Ты перешла красную линию), zashkvar etymology (prison slang → internet → youth), Rus utanc kulturu, internet argo evrimi, 2 dialogues, 8 drills, 2 cultural notes, summary box |
| 2026-01-26 | MAIN REPO page_55.html | **DENSIFIED** - YouTuber Kulturu ve Video Outro (54.6KB) ✅ GOLD STANDARD - Social media vocabulary (подписаться/лайкнуть/колокольчик/донат/ролик/стрим/блогер/контент/хайп), Imperative mood for CTAs (formal vs informal: подпишитесь/подпишись), reflexive verbs подписаться НА + Acc / отписаться ОТ + Gen full conjugation, "Всех обнял" performative past tense phenomenon, обнять full conjugation, reaction slang (Нифига себе!/Ничоси!/Офигеть!/Круто!/Огонь!/Класс!/Отстой!), platform slang (Телега/ВК/Инста/Ютубчик), streamer culture (донат/стрим/Го в стрим!), video outro complete script pattern, "Фига" etymology (incir → el hareketi → hicbir sey → sasirma), Rus YouTube kulturu, 2 dialogues, 8 drills, 2 cultural notes, summary box |
| 2026-01-26 | MAIN REPO page_56.html | **DENSIFIED** - Video II: The Egoist / Kisilik ve Ozguven (57.5KB) ✅ GOLD STANDARD - Personality adjectives (эгоист/эгоистка, уверенный, скромный, гордый, наглый, дерзкий), age specifiers (ровно/точно/почти/примерно/около/уже/всего), short-form adjectives for personality (уверена/горда/скромна/честна), frequency adverbs (всегда/часто/иногда/редко/никогда) + double negative rule, vahtovik culture (вахтовик/вахта/на вахте), relationship status questions (Есть парень?/Ты свободна?/Ты замужем?), reaction expressions politeness levels (Ого→Нифига себе→Охуеть), personality test questions (Какая ты по характеру?/Ты себя любишь?), confidence expressions (Я знаю себе цену/Скромность не моя черта), видеться reflexive conjugation, vahtovik relationship dynamics cultural note, egoist vs confident Russian perspective cultural note, 2 dialogues, 8 drills, 2 cultural notes, summary box |
| 2026-01-26 | MAIN REPO page_57.html | **DENSIFIED** - Na Vid: Gorunus ve Yas Tahmini (54.6KB) ✅ GOLD STANDARD - Appearance vocabulary (на вид/выглядеть/внешность/возраст/образ/костюм), "На вид" construction patterns (На вид где-то 25/На вид лет 30/Сколько мне на вид?), выглядеть conjugation table (выглядишь/выглядит/выглядим), comparative forms (моложе/старше) with age difference patterns (на три года моложе), cosplay vocabulary (косплей/косплеер/образ/персонаж/переодеваться), "Непривычно" usage + привыкать/привыкнуть full conjugation К + Dative, mysterious answers (Может быть и так.../Кто знает.../Посмотрим), appearance compliments (Ты выглядишь моложе своих лет!/Тебе идёт этот цвет!), Slav age perception culture, Russian cosplay culture (Comic Con Russia, DIY costumes, VK communities), 2 dialogues, 8 drills, 2 cultural notes, summary box |
| 2026-01-26 | MAIN REPO page_58.html | **DENSIFIED** - Sonrasi Planlar ve Sosyal Medya Promosyonu (63.8KB) ✅ GOLD STANDARD - Social media vocabulary (после/ссылка/описание/бот/канал/подписаться/оставить/закрытый клуб/донат/промокод/скидка/скинуть), После + Genitive patterns with pronouns table, оставить full conjugation (both aspects), вообще multi-meaning usage (hic/genel olarak/zaten/aslinda), скинуть slang verb conjugation (argo "atmak"), social media platform vocabulary (канал/группа/личка/сторис/рилс/стрим), monetization vocabulary (донат/спонсор/реклама/интеграция/закрытый клуб), YouTuber/influencer standard phrases (Подпишись на канал!/Ссылку оставила в описании!/Вступай в мой закрытый клуб!/Всех обнял!), plan-making patterns (У тебя после есть планы?/Планов вообще нет/Может погуляем?/Да пошла!), Rus sosyal medya ekosistemi (VK/Telegram/Odnoklassniki), Zakrytyy Klub monetization model cultural note, 2 dialogues, 8 drills, 2 cultural notes, summary box |
| 2026-01-26 | MAIN REPO page_59.html | **DENSIFIED** - Rationalization & Body Compliments (59.2KB) ✅ GOLD STANDARD - Gulyat dual meaning (walking vs cheating), "Nalevo" idiom (sola gitmek = aldatmak), izmena/izmenyat + Dative conjugation, rationalization patterns (Eto ne izmena/Nichego ser'yoznogo/Prosto.../Mezhdu nami nichego net), diminutive suffixes -ENK-/-ONK- (khudaya→khuden'kaya), body compliment spectrum (stroynaya→khudaya→toshchaya, pyshnaya→polnaya→tolstaya), vesit' conjugation (kilo sorma), rost (boy), figura/telo vocabulary, weight/height discussion patterns, paranoit' argo verb, vyponyat'/vypolnit' conjugation, gulyat culture historical context, Rus body standards cultural note, 2 dialogues, 8 drills, 2 cultural notes, summary box |
| 2026-01-26 | MAIN REPO page_60.html | **DENSIFIED** - Fun Facts ve Sohbet Baslangiclar (58.7KB) ✅ GOLD STANDARD - Kstati transition word usage patterns (kstati, mezhdu prochim, kstati govorya, k slovu), fun fact patterns ("Ty znala, shto...?", "Okazyvayetsya...", "Interesnyy fakt:"), reaction expressions (Ser'yozno?/Pravda?/Ne mozhet byt'!/Nichego sebe!/Ofiget'!/Da ladno!/Vryosh'!), large numbers (hundreds, thousands, millions), height/weight vocabulary (rost, ves, metr, santimetr), approximate vs exact expressions (primerno/okolo + Gen vs tochno/rovno), personal stat questions (age/height/weight/zodiac), Russia trivia (11 time zones, Baikal, "kayf" from Turkish "keyif"!), Turk-Rus linguistic connections, "Chto? Gde? Kogda?" trivia culture, VK/Telegram viral fact pages, 2 dialogues, 8 drills, 2 cultural notes, summary box |
| 2026-01-26 | MAIN REPO page_61.html | **DENSIFIED** - Nostalji ve Is Hayati (54.3KB) ✅ GOLD STANDARD - Nostalgia/work vocabulary (detstvo/vospominaniya/ran'she/dvor/shalash/stroyka/biznes/rabota/zarplata), "V + Prepositional" time expressions (v detstve/v shkole/v yunosti/v devyanostykh), irregular verb лазить full conjugation (ya lazhu - z→zh mutation), reflexive possessive свой (svoy/svoya/svoyo/svoi) gender agreement, свой vs мой distinction (independence vs simple ownership), "Pomnish'...?" nostalgia opener pattern, помнить full conjugation, "lyubit' + infinitive" construction, classic nostalgia expressions (Ran'she bylo luchshe/Khoroshie byli vremena/Ekh, molodost'!/Nostal'giya nakatila), work conversation patterns (Kem rabotayesh'?/U tebya svoy biznes?/Gde rabotayesh'?), agreement expressions (Podderzhivayu!/Tochnyak!/Blya, da!), dvorovaya kultura cultural note (Soviet courtyard culture, unsupervised play, shalash building), "svoy biznes" cultural note (post-Soviet entrepreneurship, status symbol, 90s chaos), 2 dialogues, 8 drills, 2 cultural notes, summary box |
| 2026-01-26 | MAIN REPO page_62.html | **DENSIFIED** - Fiziksel Talimatlar ve Pozisyon (44.1KB) ✅ GOLD STANDARD - Instrumental Case for body parts (рукой/ногой/коленями/головой/спиной/локтями/пальцами), position verbs (опереться/держаться/наклониться/повернуться/лечь/сесть/встать/согнуть/раздвинуть), опереться reflexive conjugation with НА + Accusative, Imperative mood review table (обопрись/держись/наклонись/ляг/сядь/встань - irregular forms highlighted), car vocabulary (сидушка argo/сиденье resmi/заднее сиденье/подголовник/руль), room vocabulary (кровать/диван/стена/пол/потолок), full position instruction sentences for car and bedroom scenarios, approval expressions (Удобно?/Так хорошо?/Тебе нравится?/Представляешь?), "Представляешь?" flirt phenomenon cultural note, Rus araba mahremiyet kulturu cultural note, 2 dialogues, 8 drills, 2 cultural notes, summary box |
| 2026-01-26 | MAIN REPO page_63.html | **DENSIFIED** - Kavga Onleme ve Konu Degistirme (51.3KB) ✅ GOLD STANDARD - Conflict/argument vocabulary (поругаться/ругаться/ссориться/злиться/обижаться/мириться/успокоиться), "Пусть + 3rd person" construction for indifference (Пусть злится/Пусть обижается/Пусть делает что хочет), Зачем vs Почему distinction (purpose vs reason), topic-changing expressions (Проехали/Забей/Зачем мы об этом?/Давай сменим тему), поругаться past tense conjugation with gender, злиться present tense conjugation + НА + Accusative, успокоиться future tense conjugation + imperative, calming phrases (Давай успокоимся/Давай без нервов/Не заводись), reconciliation expressions (Давай помиримся/Мир?/Извини/Прости меня), technology vocabulary (гуглить/бот/нейросеть/прямо в телеграме), "Забей" etymology (civi cak → bosver), "Проехали" etymology (arabayla gectik → konu kapandi), Rus kavga kulturu cultural note, 2 dialogues, 8 drills, 2 cultural notes, summary box |
| 2026-01-26 | MAIN REPO page_64.html | **DENSIFIED** - Kiyafet ve Iltifatlar / Clothing & Compliments (44.7KB) ✅ GOLD STANDARD - Clothing verbs снимать/снять vs надевать/надеть vs одевать/одеть distinction, reflexive -ся verbs for clothing problems (не снимается/не застёгивается), "Вот что значит..." irony construction, clothing vocabulary (платье/юбка/брюки/лифчик/трусики/колготки/чулки), body compliment patterns (У тебя красивая фигура/Ты такая стройная/Какие длинные ноги!), size expressions (Это мне мало/велико/как раз), body part vocabulary (талия/бёдра/грудь/попа/ноги), fitting room phrases (Где примерочная?/Можно примерить?), full conjugation tables for снимать/снять and надевать/надеть, Imperative forms (Сними!/Надень!/Разденься!), Rus kiyafet ve gorunum kulturu cultural note, Nadyet' vs Odet' dilbilgisi takintisi cultural note, 2 dialogues (soyunma odasi + flort), 8 drills, 2 cultural notes, summary box |
| 2026-01-26 | MAIN REPO page_65.html | **DENSIFIED** - Ihanet Felsefesi ve Ahlaki Yargilama (52.9KB) ✅ GOLD STANDARD - Betrayal vocabulary (измена/изменять/изменник/верность/доверие/предательство/предавать), emotional reaction vocabulary (разочарование/обида/разрыв/расставание/непростительно/недопустимо/оправдание/месть), осуждать/осудить full conjugation (moral condemnation), прощать/простить full conjugation + ACC + ЗА + ACC structure, предавать/предать IRREGULAR verb full conjugation, abstract noun suffixes -ОСТЬ (feminine: верность/честность/ревность) vs -СТВО (neuter: предательство/чувство), "При себе" construction (physical/emotional "keeping someone"), "Не нужно + infinitive" vs "Не надо" vs "Нельзя" vs "Не смей" prohibition strength ladder, key judgment expressions (Я категорично осуждаю измену/Это предательство доверия/Верность - основа отношений/Это непростительно), Russian proverb "Один раз изменил - всю жизнь будет изменять", Sovyet donemi "izmena rodine" mirasi ve kelime agirigi, affetme vs affetmeme Rus perspektifi + Proshchyonoye voskresen'ye (Affetme Pazari), "prostit'" etimolojisi (prostoy = basit), 2 dialogues (ihanet itirafi + arkadaslar arasi tartisma), 8 drills, 2 cultural notes, summary box |
| 2026-01-26 | MAIN REPO page_66.html | **DENSIFIED** - Ayrilik Mesaji / Breakup Text Protocol (44.8KB) ✅ GOLD STANDARD - Breakup vocabulary (расставаться/расстаться, бросать/бросить, уходить/уйти), messaging vocabulary (сообщение/написать/отправить/заблокировать), honesty adverbs (честно/искренне), closure expressions (точка/конец/окончательно), расставаться full conjugation table (reflexive + С + Instrumental), бросить full conjugation with С→Ш mutation (брошу), breakup text templates (direct: "Мы расстаёмся. Это моё окончательное решение", explanatory: "Дело не в тебе", boundary-setting: "Больше не пиши мне"), Russian texting abbreviations (спс/пж/норм/хз/имхо), parenthesis culture ()/)))/(/((( for emotions, Rus "ghost yapmak" cultural taboo (Исчезнуть = karaktersizlik), breakup medium appropriateness (mesaj vs telefon vs yuzyuze), "Это из-за него/неё?" expected question pattern, 2 dialogues (text exchange + in-person breakup), 8 drills, 2 cultural notes, summary box |
| 2026-01-26 | MAIN REPO page_67.html | **DENSIFIED** - Merak ve Beklenti / Curiosity & Anticipation (47.9KB) ✅ GOLD STANDARD - Curiosity expressions (Интересно.../Любопытно.../Мне интересно...), showing/proving verbs (показать/доказать) full conjugation, Чтобы + past tense subjunctive construction, Пока не + Perfective construction (until not), Интересоваться + Instrumental Case, Распинаться idiom (dil dökmek, Türkçeden!), skepticism expressions (Да ладно!/Врёшь!/Посмотрим), anticipation vocabulary (ждать/предвкушать/надеяться), "wait and see" phrases, Russian skepticism culture, 2 dialogues, 8 drills, 2 cultural notes, summary box |
| 2026-01-26 | MAIN REPO page_68.html | **DENSIFIED** - Hayat Felsefesi / Life Philosophy (50.8KB) ✅ GOLD STANDARD - Life philosophy vocabulary (жизнь/момент/мгновение/смысл/цель/мечта/счастье/свобода/душа/судьба), жить/прожить aspect pair full conjugation tables (live continuously vs complete a period), наслаждаться + Instrumental Case construction (жизнью/свободой/моментом), Пока + Present Tense "while" construction (Пока молодая - гуляй!), Надо vs Нужно vs Следует modal comparison (informal→formal scale), short-form adjectives (молода/свободна/счастлива/жива/готова), ловить/поймать aspect pair with В→ВЛ mutation (ловлю), Carpe Diem expressions (Живи сейчас!/Лови момент!/Один раз живём!/Жизнь одна!), fatalism expressions (Что будет, то будет/Такова судьба/Будь что будет!), "кайф" etymology (from Turkish "keyif"!), Russkaya Dusha cultural note (deep + melancholic + hedonist + fatalist blend), Soviet vs post-Soviet hedonism attitudes, 2 dialogues (cafe philosophy + sister advice), 8 drills, 2 cultural notes, summary box |
| 2026-01-26 | MAIN REPO page_69.html | **DENSIFIED** - Dijital Kapaniş / Digital Endings & Freedom (42.4KB) ✅ GOLD STANDARD - Digital action verbs (заблокировать/удалить/отписаться) full conjugations, digital cleanup protocol (блок→удаление→отписка), freedom/celebration expressions (Свободна!/Наконец-то!/Избавилась!), В кармане construction (in the pocket = secured), Russian digital breakup culture, Telegram/VK blocking mechanics, "чистка" digital cleanse ritual, 2 dialogues, 8 drills, 2 cultural notes, summary box |
| 2026-01-26 | MAIN REPO page_70.html | **DENSIFIED** - Gece Hayatı / Nightlife & Partying (43.5KB) ✅ GOLD STANDARD - Nightlife vocabulary (клуб/бар/тусовка/дискотека), тусоваться conjugation (reflexive party verb), танцевать conjugation (-ЕВАТЬ pattern with Е→У mutation), пить/выпить/напиться (drinking aspect trio), time expressions with Instrumental Case (утром/вечером/ночью), Каждый + noun patterns, slang evaluation spectrum (круто→офигенно→охуенно), Russian nightlife culture, 2 dialogues, 8 drills, 2 cultural notes, summary box |
| 2026-01-26 | MAIN REPO page_71.html | **DENSIFIED** - Fotoğraf Kültürü ve Selfie / Photo Culture & Selfie Slang (82.8KB) ✅ GOLD STANDARD - фоткать vs фотографировать (slang vs formal), фоткать/сфоткать full conjugation tables, сфоткаться reflexive (selfie/together), селфи vs себяшка (English loan vs Russian derivation), фотошопить conjugation (П→ПЛ mutation), выложить/запостить social media verbs (СТ→Щ mutation), photo quality expressions (чёткая/размытая/в фокусе), photo compliments (Огонь!/Красотка!/Бомба!), тусовщица party girl identity, ложиться/лечь sleep verbs (лечь irregular!), сова vs жаворонок chronotypes, photo request patterns (Сфоткай меня!), Russian selfie culture, 2 dialogues, 8 drills, 2 cultural notes, summary box |
| 2026-01-26 | MAIN REPO page_72.html | **DENSIFIED** - Öğrenci Hayatı ve Umursamazlık / Student Life & Indifference (63KB) ✅ GOLD STANDARD - учиться/изучать distinction (to study vs to learn), Dative + indifference expressions (мне пофиг/мне по барабану/мне всё равно/мне фиолетово), student slang (халява/шпаргалка/списывать/домашка/зачёт/сессия), отрываться/оторваться conjugation (party hard), халява ritual (зачётка на подоконнике), double negative rule (никогда не), formal register (мне безразлично), indifference politeness scale, Russian student superstitions, 2 dialogues, 8 drills, 2 cultural notes, summary box |
| 2026-01-26 | MAIN REPO page_73.html | **DENSIFIED** - İş ve Para / Jobs & Money (64.4KB) ✅ GOLD STANDARD - работать/зарабатывать conjugation tables, beauty industry jobs with feminine forms (-ИСТ→-ИСТКА pattern: визажист→визажистка, стилист→стилистка), money expressions with много/мало + Genitive, financial hardship expressions (Денег нет/Сижу на мели/Не хватает), independence expressions (я одна/сама по себе), подработка side hustle culture, informal work vocabulary (халтура/левак/калым), payment frequency adverbs introduction, beauty industry career paths, Russian economic reality post-2014, 2 dialogues, 8 drills, 2 cultural notes, summary box |
| 2026-01-26 | MAIN REPO page_74.html | **DENSIFIED** - Ödeme ve Sosyal Medya / Payment Terms & Social Media (60KB) ✅ GOLD STANDARD - Payment frequency adverbs (помесячно/понедельно/ежедневно/раз в неделю), платить full conjugation (Т→Ч mutation: плачу), Instagram/VK terminology (актуальные=highlights, сторис, подписчики, лента), birthday expressions (С днём рождения!), желать + Genitive Case construction, поздравлять + ACC + С + Instrumental construction, С + Instrumental celebration pattern, age politeness norms, influencer payment models, Russian birthday traditions, 2 dialogues, 8 drills, 2 cultural notes, summary box |
| 2026-01-26 | MAIN REPO page_75.html | **DENSIFIED** - Onay ve Sevgi Hitapları / Approval & Terms of Endearment (77.4KB) ✅ GOLD STANDARD - пойдёт/сойдёт/подойдёт approval scale, годиться conjugation + для + Genitive, approval intensity scale (сойдёт→превосходно), terms of endearment categories (animal: зайка/котёнок/рыбка, nature: солнышко/звёздочка, adjective: любимая/дорогая), diminutive suffixes (-шка/-очка/-ечка/-ышко/-ёнок), gender variations (милашка→милаш, красавица→красавчик), -АШКА slang suffix (симпатяшка/няшка/мимишка), compliment verbs поразить/впечатлить/удивить/очаровать full conjugations, admiration verbs восхищаться/любоваться + Instrumental, обожать (stronger than любить), "Ты меня поразила" key phrase, Russian endearment culture, "пойдёт" neutral approval culture, 2 dialogues, 8 drills, 2 cultural notes, summary box |
| 2026-01-26 | MAIN REPO page_24.html | **DENSIFIED** - Oral Mekanikleri / Oral Mechanics (40.6KB) ✅ GOLD STANDARD - Oral verbs expanded vocabulary (лизать/сосать/глотать/целовать/кусать/дуть/ласкать/облизывать/заглатывать/кончать/стонать/дрочить), лизать conjugation with З→Ж consonant mutation, глотать regular conjugation + aspect pair проглотить, Comparative adjectives (быстрее/медленнее/глубже/нежнее/сильнее) for speed/intensity control, глубже irregular form (К→Ж mutation), Instrumental Case for body parts (языком/губами/рукой/пальцами/зубами/горлом), technique directives table, sensory feedback expressions (Ты сладкая/Как хорошо пахнет/Ты такая мокрая), orgasm/final expressions (Кончаю!/Я близко/Не останавливайся!/Глотай/Выплюни), Russian intimate communication culture, "глотать или нет" discussion etiquette, 2 dialogues, 6 drills, 2 cultural notes, summary box |
| 2026-01-26 | MAIN REPO page_25.html | **DENSIFIED** - Nightlife ve Lojistik / Nightlife & Logistics (45.0KB) ✅ GOLD STANDARD - Nightlife vocabulary (клуб/бар/тусовка/вечеринка/танцпол/диджей/вышибала/фейсконтроль/гардероб), isolation phrases (Тут слишком громко/Пошли на улицу/Хочешь подышать свежим воздухом?), vape culture (под/тяга/вкус) as conversation opener, drink vocabulary (пиво/вино/водка/шампанское/коктейль/шот), bar ordering phrases (Два пива/Я угощаю/За знакомство!/Счёт пожалуйста), пить irregular conjugation (пью/пьёшь/пьёт), intoxication levels scale (трезвая→подвыпившая→навеселе→пьяная→в говно→в хлам→в отключке), motion verbs пойти vs поехать distinction (walking vs vehicle), home invitation phrases (Поехали ко мне/Хочешь зайти на чай?), вызвать conjugation for taxi, Russian toast culture (За знакомство!/За любовь!), "зайти на чай" universal excuse cultural note, 2 dialogues, 6 drills, 2 cultural notes, summary box |
| 2026-01-26 | MAIN REPO page_26.html | **DENSIFIED** - Survival Russian / Hayatta Kalma Ruscasi (48.1KB) ✅ GOLD STANDARD - Emergency vocabulary (помогите/полиция/скорая/врач/больница/аптека/опасность), 112 emergency system explanation, Мне нужен/нужна/нужно construction with gender agreement, Imperative mood emergency commands (Помогите!/Вызовите полицию!/Пожар!/Держите вора!), police interaction phrases (Я туристка из Турции/Я не понимаю/Вот мой паспорт), direction words (прямо/направо/налево/здесь/там/рядом/напротив), taxi phrases, theft/loss expressions (У меня украли.../Я потеряла...), medical emergency phrases (Мне плохо/У меня болит.../У меня аллергия), Russian smile culture proverb, police/authority culture, 2 dialogues, 8 drills, 2 cultural notes, summary box |
| 2026-01-26 | MAIN REPO page_27.html | **DENSIFIED** - Social Conflict / Sosyal Catisma (44.8KB) ✅ GOLD STANDARD - Indifference scale (всё равно→плевать→пофиг→похуй), Dative Case with indifference expressions, НА + Accusative for targets (Мне плевать на это), "Что за...?" construction for outrage, "Всё про..." construction (Здесь всё про секс), rejection expressions politeness scale (Извини но нет→Забудь→Отвали→Иди нахуй), бесить conjugation with И→Я mutation, достать perfective usage, фигня/херня/хуйня rudeness scale, Russian directness culture, 2 dialogues, 8 drills, 2 cultural notes, summary box |
| 2026-01-26 | MAIN REPO page_28.html | **DENSIFIED** - Gossip & Dismissal / Dedikodu ve Kovma (46.3KB) ✅ GOLD STANDARD - Slang for women (тёлка/баба/чика/девка/стерва/сучка/красотка) with severity levels, Imperative mood formation rules, dismissal phrases (забудь/успокойся/отстань/уйди/отвали/заткнись), dismissal severity scale (kibar→sert→mat), начать perfective conjugation (past + future), завидовать + Dative conjugation, status expressions (Я тут главная/Знай своё место), gossip patterns (Ты слышала?/Говорят что.../Между нами...), истеричка and emotional labels, Russian female friendship culture, 2 dialogues, 8 drills, 2 cultural notes, summary box |
| 2026-01-26 | MAIN REPO page_29.html | **DENSIFIED** - Rejection & Ranting / Ekilme Durumlari (37.2KB) ✅ GOLD STANDARD - Flaking vocabulary (кидать/кинуть/кинула/кидалово), abandonment verbs (бросать/бросить/бросила), betrayal verbs (предавать/предать/предала), deception verbs (обманывать/обмануть/обманула), кинуть full conjugation table (impf/perf), бросить conjugation with Ш mutation (брошу), предать irregular conjugation (предам/предашь/предаст/предадим/предадите/предадут), rhetorical questions (Из-за чего? + Genitive, Как же...?, Что за...?), Пиздец spectrum (negative/surprise/intensity/finality/admiration), curse word severity scale (Блин→Чёрт→Блядь→Пиздец→Полный пиздец), проехали for acceptance, escalation ladder 5 levels, Russian "flaking" culture (может быть = probably no), мат etiquette and safe alternatives (Капец!/Ёлки-палки!), 2 dialogues (The Flake + The Breakup), 4 drills, 2 cultural notes, summary box |
| 2026-01-26 | MAIN REPO page_30.html | **DENSIFIED** - Threesome & Proxy / Araci Olma (35.7KB) ✅ GOLD STANDARD - Threesome vocabulary (тройничок/трое/втроём), proxy request structure ([Kisi] + хочет + [Nesne] + от + [Kisi-Gen]), хотеть irregular conjugation (хоч- singular vs хот- plural), number derivatives table (двое/трое/четверо/пятеро + вдвоём/втроём/вчетвером/впятером), persuasion idioms (У меня денег как воды/Деньги не проблема/Я заплачу за всё), negative response stoppers (Хватит ныть/Не начинай/Успокойся/Расслабься), consent questions (Ты согласна?/Тебе нормально?/Ты уверена?/Хочешь попробовать?), positive consent responses (Да согласна/Давай попробуем/Почему бы и нет?), negative consent responses (Нет не хочу/Это не для меня/Я не готова), proxy communication culture, consent importance in Russian relationships, 2 dialogues (The Proposal + The Persuasion), 4 drills, 2 cultural notes, summary box |
| 2026-01-26 | MAIN REPO page_31.html | **DENSIFIED** - Past Tense & Interrogation / Gecmis Zaman Sorgulama (36.4KB) ✅ GOLD STANDARD - БЫТЬ past tense gender agreement (был/была/было/были), У + Gen + был/была possession structure, Сколько было? quantity questions, interrogation patterns (У тебя был секс?/Сколько было парней?/Когда был первый раз?/С кем был первый раз?), emphasis patterns (Так ты что...?/Даже...не...?/Неужели...?), diminutive suffixes table (-чик/-ик/-ок/-ка/-ки: палец→пальчик, рот→ротик, язык→язычок, губа→губки, нога→ножка, рука→ручка), diminutive tone shifts (sevgi vs alay), experience level expressions (У меня не было опыта→У меня много опыта), boundary-setting phrases (Это не твоё дело/Это личное/Я не хочу об этом говорить), Russian directness in intimate questions, diminutive usage context, 2 dialogues (The Interview + Setting Boundaries), 4 drills, 2 cultural notes, summary box |
| 2026-01-26 | MAIN REPO page_32.html | **DENSIFIED** - Bar & Etiquette / Bar Adabi (49.9KB) ✅ GOLD STANDARD - Можно construction patterns (permission/requests), ordering politeness scale (Будьте добры→пожалуйста→Мне→Дай), quantity expressions with gender (один/одна/одно, два/две), За + Accusative toasting patterns (За здоровье!/За знакомство!/За любовь!/За нас!/За встречу!/За удачу!/За прекрасных дам!), угостить conjugation (treat/offer drinks) + ACC + INST structure, short-form adjectives (готов/готова, рад/рада, занят/занята, свободен/свободна, пьян/пьяна), hesap isteme patterns (Счёт пожалуйста/Можно счёт?/Сколько с меня?), payment methods (наличными/картой/переводом), bar vocabulary (бармен/меню/счёт/чаевые/коктейль/шот/бокал/рюмка), Можно vs Нельзя distinction, Russian toast culture (bos kadehle tost yasak, goz goze, ucuncu tost ask icin), bar etiquette (bahsis %10, Сдачу оставьте, masa servisi vs bar), 2 dialogues (At the Bar + Toasting), 6 drills, 2 cultural notes, summary box |

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

*Document Version: 58.0*
*Last Updated: 2026-01-26*
*Project Status: 🛑 PLAYBOOK FROZEN - Sayfa 01-19 tamamlandı. Main repo page_17-32 ve page_46-75 densified. ⚠️ KALAN: Main repo pages 33-45 hala SEVERE (3-6KB) - densification gerekli. Pages 01-16 INADEQUATE.*
