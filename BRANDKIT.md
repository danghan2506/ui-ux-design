# PINGO — Brand Identity & Visual System Guidelines (`BRANDKIT.md`)

> **Brand Name:** PINGO  
> **Category:** Gamified AI English Phrase & Speaking Reflex Mobile Application (iOS & Android)  
> **Brand Positioning:** Playful Tactile Edutainment meets Swiss Geometric Clarity & Studio Audio  
> **Primary Tagline:** *"Catch the lingo. Spark the chat."*  
> **Design System Companion:** See [DESIGN.md](file:///d:/projects/ui-ux/DESIGN.md) for Google Stitch screen generation rules and UI component specifications.

---

## 1. Brand Strategy & Core Philosophy

### 1.1 Why PINGO Exists
Traditional English learning applications force learners into a false dichotomy: either childish cartoon mascots focused on isolated single words, or rigid academic test-prep dashboards that induce speaking anxiety. **PINGO** bridges this divide for Gen Z, university students, and young professionals by turning **native English phrases** and **live AI speaking reflex** into a fast, pressure-free daily game—without any childish cartoon characters.

Every daily session follows the signature **5-Minute "Learn-then-Speak" Loop**:
1. **Phase 1 — Phrase Catch (Daylight Play Surface, `#FBF9F5`):** Learners play 3 to 5 tactile mini-games (interlocking phrase jigsaw, scenario matching, rhythm chunk assembly) to absorb authentic idioms and sentence blocks.
2. **Phase 2 — AI Voice Reflex Studio (Cozy Night Surface, `#141318`):** Immediately after unlocking the day's phrases, the screen shifts into an intimate dark-mode audio studio. For 120 seconds (`02:00`), learners jump into a lively voice chat with PINGO AI and must naturally speak the exact target phrases they just learned to trigger combo multipliers (`COMBO 4x`) and keep their daily streak alive.

### 1.2 Etymology of "PINGO"
The name **PINGO** encodes three interconnected layers of meaning:
1. **PING** *(Conversational Reflex & Acoustic Signal)*: Inspired by a fast rally in *Ping-Pong* and an acoustic sonar ping—hearing a conversational cue and bouncing back a spoken response without hesitation.
2. **LINGO** *(Living, Idiomatic Language)*: Real-world phrases, cultural expressions, and natural sentence chunks used by native speakers today.
3. **BINGO!** *(The Gamified Win Moment)*: The instant tactile satisfaction when a spoken phrase locks into place during a live conversation.

### 1.3 Brand Personality Matrix
| Trait | What PINGO Is | What PINGO Is Never |
| :--- | :--- | :--- |
| **Playful yet Mature** | Witty, tactile, game-driven, culturally sharp | Childish cartoon animals, goofy mascots, nursery-school UI |
| **Architectural & Warm** | Crisp Swiss monogram geometry (`P`) + warm paper tones (`#FBF9F5`) | Cold corporate SaaS or messy AI clip-art |
| **Action-Oriented** | Focused on speaking out loud within 2 minutes | Passive grammar theory or endless multiple-choice tables |
| **Studio-Crafted** | Disciplined typography (`Satoshi` + `Fraunces` + `JetBrains Mono`) | Generic AI neon purple/blue gradients or `Inter` defaults |

---

## 2. Logo System & Monogram Architecture ("The Ping-Loop `P`")

### 2.1 Symbolic Monogram Concept (`Monogram + Meaning`)
The **PINGO Monogram (`P`)** is a pure, minimal typographic mark constructed from two modular geometric primitives that directly express the product's **"Phrase Block + Voice Ping"** mechanic:

```
[Vertical Phrase Pillar (Stem)] + [Acoustic Speech Loop + Ping Node (Bowl)] = THE PINGO "P" MONOGRAM
```

1. **The Stem — The Phrase Block:** A bold vertical rounded capsule (`width: 18px`, `height: 64px`, `rx: 9px`) on the left, representing a solid structural sentence block (Phase 1 input).
2. **The Bowl — The Acoustic Speech Loop:** A detached, bold semicircular loop (`stroke-width: 16px`, `stroke-linecap: round`) that curves outward from the stem to form the upper counter of the letter **`P`**, with a subtle bottom-left speech-tail notch.
3. **The Core — The Ping Dot:** Floating at the exact optical center of the `P`'s counter is a solid circle (`r: 6px`) that acts as an acoustic signal origin—radiating voice energy when active in the UI.

### 2.2 Geometric Construction Grid (24×24 Module System)
- **Canvas Grid:** `24 × 24` modular units (`120px × 120px` master vector).
- **Left Vertical Stem:** `X: 5..8.5`, `Y: 4..20`, pill radius `1.75 units`.
- **Outer Bowl Radius:** Centered at `(13, 10.5)` with outer radius `R_out = 6.5 units` and inner counter radius `R_in = 3.25 units`.
- **Optical Gap (Negative Space Cut):** A crisp `1.5-unit` vertical channel separates the left stem from the right bowl, giving the `P` stencil precision and contemporary architectural tension.
- **Central Ping Node:** Circle centered at `(13, 10.5)` with radius `R_dot = 1.4 units`.
- **Minimum Clear Space:** Equal to `0.25 ×` the height of the `P` monogram on all four sides.
- **Minimum Render Size:** `18px × 18px` for mobile status badges; `36px` height for full horizontal lockup.

### 2.3 Production SVG Assets

#### A. Primary Horizontal Lockup (Daylight Surface `#FBF9F5`)
```xml
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 360 100" width="360" height="100" fill="none">
  <!-- Daylight Surface Preview -->
  <rect width="360" height="100" rx="24" fill="#FBF9F5"/>
  
  <!-- Tactile 3D App Tile Base -->
  <rect x="16" y="18" width="68" height="68" rx="20" fill="#B34E24"/>
  <rect x="16" y="14" width="68" height="68" rx="20" fill="#E06D3B"/>
  
  <!-- Minimalist Geometric "P" Monogram -->
  <!-- 1. Left Vertical Phrase Pillar (Stem) -->
  <rect x="31" y="27" width="12" height="42" rx="6" fill="#18181B"/>
  <!-- 2. Right Acoustic Speech Loop (Bowl of P) -->
  <path d="M48 27H54C62.8366 27 70 34.1634 70 43C70 51.8366 62.8366 59 54 59H48V49H54C57.3137 49 60 46.3137 60 43C60 39.6863 57.3137 37 54 37H48V27Z" fill="#18181B"/>
  <!-- 3. Optical Center Ping Dot -->
  <circle cx="53.5" cy="43" r="4" fill="#FBF9F5"/>
  
  <!-- PINGO Geometric Wordmark (Satoshi Black) -->
  <text x="102" y="64" fill="#18181B" font-family="'Satoshi', 'Outfit', sans-serif" font-weight="900" font-size="48" letter-spacing="-0.03em">PINGO</text>
  <circle cx="268" cy="56" r="5" fill="#E06D3B"/>
</svg>
```

#### B. Standalone `P` Monogram on Cozy Night Studio Surface (`#141318`)
```xml
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 120 120" width="120" height="120" fill="none">
  <!-- Cozy Night Obsidian Studio Background -->
  <rect width="120" height="120" rx="32" fill="#141318"/>
  
  <!-- Concentric Acoustic Studio Rings -->
  <circle cx="60" cy="60" r="48" stroke="#E06D3B" stroke-opacity="0.20" stroke-width="1.5" stroke-dasharray="5 5"/>
  <circle cx="60" cy="60" r="38" stroke="#E06D3B" stroke-opacity="0.35" stroke-width="1.5"/>
  
  <!-- Minimalist "P" Monogram -->
  <!-- 1. Left Stem -->
  <rect x="34" y="30" width="16" height="60" rx="8" fill="#F5F3EF"/>
  <!-- 2. Right Bowl of P -->
  <path d="M56 30H65C77.7025 30 88 40.2975 88 53C88 65.7025 77.7025 76 65 76H56V62H65C69.9706 62 74 57.9706 74 53C74 48.0294 69.9706 44 65 44H56V30Z" fill="#F5F3EF"/>
  <!-- 3. Active Tangerine Ping Core -->
  <circle cx="64" cy="53" r="6" fill="#E06D3B"/>
</svg>
```

### 2.4 Monogram Interactive States (In-App Kinetic Behavior)
Instead of a cartoon mascot, the **`P` Monogram** acts as a kinetic precision instrument that responds to gameplay:
1. **State 01 — Static Precision (Default Light Mode):** Clean high-contrast `#18181B` stem and bowl with a stationary `#E06D3B` Ping Dot inside the counter.
2. **State 02 — Phrase Snap (Correct Word Tile Match):** The left vertical stem and right bowl briefly compress `2px` toward each other and rebound with spring physics (`stiffness: 220, damping: 18`) while the central Ping Dot flashes Moss Confirm (`#589E42`).
3. **State 03 — Voice Radar (Dark Mode AI Voice Studio):** The central Ping Dot inside the `P` bowl pulses continuously, radiating concentric **Tangerine Pop (`#E06D3B`)** sound rings synced to the user's live microphone input.

---

## 3. Adaptive Studio Color System

### 3.1 Color Philosophy
PINGO uses an **Adaptive Dual-Zone Palette** tailored to the cognitive demands of each learning phase:
- **Daylight Play Zone (`#FBF9F5` Creamy Alabaster):** Warm, tactile paper-inspired neutrals that make reading idioms, grammar chunks, and cultural notes effortless and inviting.
- **Cozy Night Studio Zone (`#141318` Obsidian):** When the 2-minute AI Voice Reflex begins, the interface dims like a professional audio booth, removing visual clutter so the learner focuses entirely on listening and speaking.
- **Singular High-Agency Accent (`#E06D3B` Tangerine Pop):** A warm, desaturated terracotta-tangerine (`HSL: 19°, 73%, 55%`) that unifies both zones. It carries enough warmth to feel joyful and game-like in Daylight Mode, and glows like an analog studio "ON AIR" signal in Cozy Night Mode.

### 3.2 Complete Color Token Specification

```css
:root {
  /* ==========================================================================
     PHASE 1: DAYLIGHT PLAY SURFACE (MINI-GAMES & PHRASE CARDS)
     ========================================================================== */
  --pingo-day-canvas: #FBF9F5;           /* Warm Alabaster primary viewport background */
  --pingo-day-surface: #FFFFFF;          /* Pure Cloud elevated card & tile fill */
  --pingo-day-subtle: #F3EFE6;           /* Recessed slot background for empty word banks */
  --pingo-day-border: #E6E1D6;           /* 2px structural card outline */
  --pingo-day-lip: #D6CFC2;              /* 4px tactile 3D bottom lip for neutral word tiles */

  /* ==========================================================================
     PHASE 2: COZY NIGHT VOICE STUDIO (2-MINUTE AI SPEAKING REFLEX)
     ========================================================================== */
  --pingo-night-canvas: #141318;         /* Cozy Night Obsidian primary studio background (NEVER #000000) */
  --pingo-night-surface: #1E1C24;        /* Plum Slate elevated card & AI prompt container */
  --pingo-night-elevated: #282530;       /* Interactive chip surface in dark studio */
  --pingo-night-border: rgba(255, 255, 255, 0.09); /* 1px whisper structural border */
  --pingo-night-lip: #0D0C10;            /* 4px tactile bottom lip for dark-mode secondary buttons */

  /* ==========================================================================
     TYPOGRAPHIC INK & HIERARCHY TOKENS
     ========================================================================== */
  --pingo-ink-primary-day: #18181B;      /* Charcoal Ink (Zinc-950 depth) for primary text on light */
  --pingo-ink-secondary-day: #71717A;    /* Muted Warm Steel for translations & hints on light */
  --pingo-ink-tertiary-day: #A1A1AA;     /* Subtle metadata & disabled states on light */

  --pingo-ink-primary-night: #F5F3EF;    /* Warm Ivory for primary text & live transcript on dark */
  --pingo-ink-secondary-night: #A1A1AA;  /* Ash Zinc for secondary labels in voice studio */
  --pingo-ink-tertiary-night: #6E6B78;   /* Muted studio timestamps & inactive cues */

  /* ==========================================================================
     SINGLE PRIMARY ACCENT — TANGERINE POP (SATURATION 73% < 80% MAX)
     ========================================================================== */
  --pingo-accent-primary: #E06D3B;       /* Tangerine Pop — Primary CTAs, P Monogram Core, Voice Orb, Streak */
  --pingo-accent-hover: #E67B4C;         /* Tactile highlight state */
  --pingo-accent-lip: #B34E24;           /* Deep Terracotta 4px 3D bottom push lip */
  --pingo-accent-tint-day: rgba(224, 109, 59, 0.14);   /* Selected phrase tile wash (Light) */
  --pingo-accent-tint-night: rgba(224, 109, 59, 0.20); /* Active target phrase glow wash (Dark) */

  /* ==========================================================================
     SEMANTIC GAME FEEDBACK TOKENS (CONTROLLED SATURATION)
     ========================================================================== */
  --pingo-feedback-success: #589E42;     /* Moss Confirm — Correct answer banner & matched phrase */
  --pingo-feedback-success-lip: #3E732D; /* 4px tactile lip for success CTA */
  --pingo-feedback-success-tint: rgba(88, 158, 66, 0.14);

  --pingo-feedback-nudge: #D4942A;       /* Honey Nudge — Gentle pronunciation or word-order retry */
  --pingo-feedback-nudge-lip: #9E6B18;   /* 4px tactile lip for retry CTA */
  --pingo-feedback-nudge-tint: rgba(212, 148, 42, 0.15);
}
```

### 3.3 Color Usage Proportions
- **Phase 1 (Daylight Play):** `75%` Creamy Alabaster & Pure Cloud (`#FBF9F5` / `#FFFFFF`), `15%` Charcoal Ink & Muted Steel (`#18181B` / `#71717A`), `10%` Tangerine Pop (`#E06D3B`).
- **Phase 2 (Cozy Night Studio):** `75%` Cozy Night Obsidian & Plum Slate (`#141318` / `#1E1C24`), `15%` Warm Ivory (`#F5F3EF`), `10%` Tangerine Pop (`#E06D3B`).

---

## 4. Typographic Architecture

### 4.1 The Three-Font Cognitive System
Every font in PINGO has a dedicated pedagogical role so the learner's brain automatically separates **UI Instructions**, **Target English Phrases**, and **Phonetic/Game Metrics**:

| Role | Font Family | Weights & Styles | Why It Works for PINGO |
| :--- | :--- | :--- | :--- |
| **1. UI, Headlines & 3D Buttons** | **`Satoshi`** | `500 Medium`, `700 Bold`, `900 Black` | Friendly geometric grotesque with wide apertures; delivers playful tactile chunkiness on buttons without feeling childish. |
| **2. Target English Phrases & Idioms** | **`Fraunces`** | `600 SemiBold`, `700 Bold`, `600 Italic` | Contemporary soft-serif with expressive warmth. Gives English idioms editorial prestige and creates a visual anchor on flashcards. |
| **3. IPA Phonetics, Timers & XP HUD** | **`JetBrains Mono`** | `500 Medium`, `700 Bold` | Crisp tabular monospace for IPA pronunciation (`/ˈspɪl ðə tiː/`), countdown clock (`02:00`), combo multipliers (`4x`), and streak counts (`14d`). |

### 4.2 Type Scale & Mobile Hierarchy
All sizes are calibrated for mobile viewports (`375px–430px` width) with fluid `clamp()` scaling:

- **Hero Phrase Display (`Fraunces Bold`):** `clamp(1.75rem, 5vw, 2.25rem)` (`28px–36px`), `line-height: 1.15`, `letter-spacing: -0.02em`. Used for the featured idiom on collectible cards.
- **Screen Mission Header (`Satoshi Black`):** `clamp(1.35rem, 4vw, 1.65rem)` (`22px–26px`), `line-height: 1.2`, `letter-spacing: -0.025em`. Used for mini-game prompts.
- **AI Dialogue & Live Transcript (`Satoshi Bold`):** `1.125rem` (`18px`), `line-height: 1.45`, `letter-spacing: -0.01em`. High legibility during real-time voice roleplay.
- **Interactive Word Tile (`Satoshi Bold` or `Fraunces SemiBold`):** `1.0rem` (`16px`), `line-height: 1.25`. Minimum `48px` touch height.
- **Translation & Cultural Context Body (`Satoshi Medium`):** `0.9375rem` (`15px`), `line-height: 1.5`, max line width `55ch`.
- **Phonetic IPA & Game HUD Pill (`JetBrains Mono Bold`):** `0.8125rem` (`13px`), `line-height: 1.0`, `letter-spacing: 0.02em`, `font-variant-numeric: tabular-nums`.
- **Tactile Primary CTA Button (`Satoshi Black`):** `0.9375rem` (`15px`), uppercase, `letter-spacing: 0.04em`.

---

## 5. Brand Voice, Tone & Microcopy Guide

### 5.1 Tone Principles
- **Encourage like a witty friend, never lecture like a textbook:** Celebrate natural spoken rhythm over stiff grammatical perfection.
- **Short, punchy, rhythm-driven sentences:** Every piece of UI copy should sound good when read aloud.
- **Ban AI corporate buzzwords:** Never use words like *"Elevate"*, *"Unleash"*, *"Seamless"*, *"Next-Gen"*, or *"Supercharge"*.

### 5.2 In-App Microcopy Dictionary
| Scenario | Generic App Copy (BANNED) | PINGO Brand Copy (APPROVED) |
| :--- | :--- | :--- |
| **Daily Notification** | "Time to complete your daily English lesson." | "Got 2 minutes? Let's catch 3 new phrases and spark a quick chat." |
| **Phase 1 → Phase 2 Shift** | "Proceed to Speaking Exercise" | "Phrases locked in! Step into the studio and drop them in live chat →" |
| **Correct Phrase Used in Voice Chat** | "Target vocabulary detected (+50 points)" | "Boom! You wove *'spill the tea'* right into the flow. +50 XP" |
| **Pronunciation Nudge** | "Incorrect pronunciation. Try again." | "Almost! Stress the first beat in *'LOW-key'* and hit it one more time." |
| **Empty Saved Phrases State** | "No bookmarks found." | "Your phrase vault is quiet. Tap the P-badge on any card to stash it here." |

---

## 6. Official 3×3 Brandkit Board Architecture

The flagship PINGO Brandkit Board follows a disciplined `3 × 3` grid (`16:10` presentation canvas on `#141318` Cozy Night Obsidian with `20px` gutters and `24px` panel corner radius):

| Row / Col | Panel Title | Visual Content & Purpose |
| :--- | :--- | :--- |
| **Panel 01 (Top-Left)** | **Logo Cover** | Geometric **`P` Monogram** + **PINGO** wordmark (`Satoshi Black`) on Creamy Alabaster (`#FBF9F5`) with generous negative space. |
| **Panel 02 (Top-Center)** | **Monogram Construction** | Architectural blueprint on `#1E1C24` illustrating `[Vertical Phrase Stem] + [Acoustic Speech Loop] + [Central Ping Node]`. |
| **Panel 03 (Top-Right)** | **Phase 1: Daylight Mini-Game UI** | iPhone mockup crop on `#FBF9F5` showing interlocking sentence puzzle blocks with `Fraunces` target idiom and 3D Tangerine Pop CTA. |
| **Panel 04 (Mid-Left)** | **Brand Essence & Tagline** | High-contrast typographic poster: *"Catch the lingo. Spark the chat."* with a tactile `"PING → SPEAK"` signal pill. |
| **Panel 05 (Mid-Center)** | **Adaptive Color System** | Tactile 3D swatch cards showing Daylight neutrals (`#FBF9F5`, `#FFFFFF`), Cozy Night studio darks (`#141318`, `#1E1C24`), and Tangerine Pop (`#E06D3B`). |
| **Panel 06 (Mid-Right)** | **Typography Specimen** | Three-tier specimen card pairing `Satoshi Black` (UI), `Fraunces Bold Italic` (Target Idioms), and `JetBrains Mono` (`/ˈlɪŋ.ɡoʊ/ • 02:00`). |
| **Panel 07 (Bottom-Left)** | **Phase 2: Cozy Night Voice Studio** | iPhone mockup crop on `#141318` showing the **`P` Monogram Voice Orb** inside a reactive Tangerine waveform ring, `02:00` timer, and live mission checklist. |
| **Panel 08 (Bottom-Center)** | **3D App Icon & Kinetic States** | Squircle iOS app icon tile featuring the geometric **`P` Monogram** with `#B34E24` 3D lip + 3 kinetic monogram states (Idle, Snap, Voice Radar). |
| **Panel 09 (Bottom-Right)** | **Tactile Game Component Strip** | Modular UI kit strip: 3D push buttons, interlocking word tiles, `14 DAY STREAK` badge, and IPA phonetic audio chip. |
