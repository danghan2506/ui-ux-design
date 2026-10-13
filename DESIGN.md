# Design System: PINGO — Gamified AI English & Voice Reflex Mobile App

## 1. Visual Theme & Atmosphere

**PINGO** is a playful, tactile, studio-crafted mobile interface that merges the effortless daily habit mechanics of **Duolingo** with the warm typographic intelligence of **Kinfolk / Readwise** and the tactile hardware precision of **Teenage Engineering / Panic Playdate**—without childish cartoon mascots.

The interface operates on an **Adaptive Dual-Zone Atmosphere ("The Learn-then-Speak Studio")**:
1. **Daylight Play Zone (Phase 1 — Vocabulary & Sentence Mini-Games):** Warm, sunlit paper-like surfaces (`#FBF9F5`) paired with crisp white 3D word tiles (`#FFFFFF`), high-contrast Charcoal Ink (`#18181B`), and expressive `Fraunces` serif idioms. The mood is inviting, pressure-free, and tactile—like arranging physical letterpress blocks on a warm desk.
2. **Cozy Night Voice Studio (Phase 2 — 2-Minute AI Speaking Reflex):** When the learner finishes assembling their daily phrases, the screen performs a smooth theatrical dim into **Cozy Night Obsidian (`#141318`)**. Elevated Plum Slate cards (`#1E1C24`) and a reactive **Tangerine Pop (`#E06D3B`)** **`P` Monogram Voice Orb** focus 100% of the user's attention on listening and speaking out loud with the PINGO AI partner.

**Atmospheric Calibration Scores (`stitch-design-taste` Spectrum):**
- **Density:** `5 / 10` (*Daily App Balanced* — generous touch spacing and zero visual clutter during timed mini-games; clean tabular HUD badges for XP, streak, and countdown timers).
- **Variance:** `7 / 10` (*Playful Asymmetric & Modular* — interlocking phrase blocks, offset typographic prompt headers, and bento-style progress summaries; strictly bans boring 3-column equal card rows).
- **Motion:** `8 / 10` (*Bouncy Spring Choreography* — tactile `-3px` 3D push buttons, spring-loaded word tile snapping, perpetual breathing voice waveform loops, and smooth surface crossfades between Daylight Play and Cozy Night Studio).

---

## 2. Color Palette & Roles

**Mandatory Calibration Rules:**
- **Single Primary Accent Constraint:** **Tangerine Pop (`#E06D3B`)** is the sole primary accent across both Daylight and Cozy Night modes. Its saturation is strictly capped at `73%` (`< 80%` threshold) to feel warm, appetizing, and studio-grade rather than harsh neon.
- **Zero Pure Black (`#000000`) Rule:** Pure `#000000` is strictly forbidden. All dark backgrounds and primary inks use calibrated warm charcoal and obsidian tones (`#141318`, `#18181B`, `#1E1C24`).
- **Zero AI Neon Glow Rule:** Purple/blue neon gradients and outer box-shadow glows are banned. Depth is communicated through crisp `2px` borders and solid `4px` 3D bottom tactile lips.

### 2.1 Phase 1 — Daylight Play Surface Tokens (Mini-Games & Phrase Cards)
- **Creamy Alabaster** (`#FBF9F5`) — Primary mobile viewport canvas for reading, flashcards, and sentence-building puzzles.
- **Pure Cloud Surface** (`#FFFFFF`) — Elevated container fill for collectible phrase cards, dialogue prompts, and draggable word tiles.
- **Recessed Sand Slot** (`#F3EFE6`) — Inset target drop-zone where learners tap or drag word tiles to complete a sentence.
- **Warm Bisque Border** (`#E6E1D6`) — `2px` structural outline around cards and unselected word tiles.
- **Tactile Tile Lip** (`#D6CFC2`) — Solid `4px` bottom lip (`0 4px 0 0 #D6CFC2`) under neutral white word tiles, giving every phrase chunk a physical keycap feel.
- **Charcoal Ink** (`#18181B`) — Primary headline, prompt, and body typography on light surfaces (Zinc-950 depth).
- **Muted Warm Steel** (`#71717A`) — Secondary text, native-language translations, and contextual usage notes.

### 2.2 Phase 2 — Cozy Night Voice Studio Tokens (2-Minute AI Speaking Reflex)
- **Cozy Night Obsidian** (`#141318`) — Primary background canvas during live AI voice roleplay sessions.
- **Plum Slate Surface** (`#1E1C24`) — Elevated container fill for AI conversational prompts, live speech transcripts, and the target-phrase mission checklist.
- **Studio Elevated Chip** (`#282530`) — Surface fill for secondary audio controls (replay slow audio, phonetic hint toggle).
- **Whisper Glass Border** (`rgba(255, 255, 255, 0.09)`) — `1px` structural hairline divider separating dark studio containers without visual noise.
- **Obsidian Tactile Lip** (`#0D0C10`) — Solid `4px` bottom lip under secondary dark-mode buttons.
- **Warm Ivory Ink** (`#F5F3EF`) — Primary text for AI prompts and user speech transcripts in dark mode.
- **Ash Zinc** (`#A1A1AA`) — Secondary labels, roleplay persona titles, and inactive transcript words.

### 2.3 Universal Accent & Semantic Feedback Tokens
- **Tangerine Pop** (`#E06D3B`) — Single primary accent used for primary 3D CTA buttons, the `P` Monogram's central Ping Dot, active voice waveform rings, progress bars, and daily streak badges.
- **Deep Terracotta Lip** (`#B34E24`) — Solid `4px` bottom 3D lip (`0 4px 0 0 #B34E24`) paired exclusively with `#E06D3B` primary buttons.
- **Soft Apricot Wash** (`rgba(224, 109, 59, 0.14)` on Light / `rgba(224, 109, 59, 0.22)` on Dark) — Highlight fill for active selected word tiles and completed voice mission chips.
- **Moss Confirm** (`#589E42` with `#3E732D` 3D lip) — Semantic confirmation state for correct sentence assembly and unlocked phrase badges.
- **Honey Nudge** (`#D4942A` with `#9E6B18` 3D lip) — Gentle semantic retry state for word-order nudges or pronunciation stress hints (replaces harsh alarmist red error banners).

---

## 3. Typography Rules

**Font Stack Architecture:**
- **Display & UI Sans-Serif:** `'Satoshi', sans-serif` — Track-tight, friendly geometric sans with generous open counters. Used for all screen headers, mission instructions, 3D button labels, and conversational transcripts.
- **Editorial Phrase Accent Serif:** `'Fraunces', serif` — Contemporary soft optical serif used **exclusively** for the target English idiom, phrasal verb, or sentence chunk being learned on flashcards and puzzle slots (e.g., *"spill the tea"*, *"lowkey a masterpiece"*). Never used for dashboard chrome, settings, or numeric tables.
- **Monospace HUD & Phonetics:** `'JetBrains Mono', monospace` — Mandatory for IPA phonetic transcriptions (`/ˈlɪŋ.ɡoʊ/`), countdown timers (`02:00`), combo multipliers (`COMBO 4x`), XP counters (`+50 XP`), and streak metrics (`14 DAYS`).
- **Strictly Banned Fonts:** `Inter`, `Roboto`, `Arial`, `Times New Roman`, `Georgia`, `Garamond`, `Palatino`, and system default UI fonts.

### 3.1 Typographic Scale & Line-Width Constraints
1. **Featured Target Phrase (`Fraunces Bold` / `Fraunces SemiBold Italic`):**
   - Size: `clamp(1.75rem, 5vw, 2.25rem)` (`28px–36px`)
   - Line Height: `1.15`
   - Letter Spacing: `-0.02em`
   - Usage: Hero idiom inside collectible flashcards and phrase-unlock celebration sheets.
2. **Mini-Game Prompt Headline (`Satoshi Black`):**
   - Size: `clamp(1.25rem, 4vw, 1.5rem)` (`20px–24px`)
   - Line Height: `1.25`
   - Letter Spacing: `-0.025em`
   - Max Width: `32ch`
   - Usage: Scenario question at the top of a puzzle screen.
3. **Live AI Studio Prompt (`Satoshi Bold`):**
   - Size: `1.125rem` (`18px`)
   - Line Height: `1.45`
   - Letter Spacing: `-0.01em`
   - Max Width: `42ch`
   - Usage: Spoken line from the AI roleplay partner inside the Cozy Night Voice Studio.
4. **Tactile Word Tile Label (`Satoshi Bold` for context words / `Fraunces Bold` for target chunk):**
   - Size: `1.0rem` (`16px`)
   - Line Height: `1.2`
   - Padding: `12px 16px`
5. **Contextual Explanation & Translation Body (`Satoshi Medium`):**
   - Size: `0.9375rem` (`15px` — strictly above the `14px` mobile floor)
   - Line Height: `1.55`
   - Max Width: `60ch`
6. **Phonetics, Timer & Combo HUD (`JetBrains Mono Bold`):**
   - Size: `0.8125rem` (`13px`)
   - Line Height: `1.0`
   - Letter Spacing: `0.03em`
   - Numeric Variant: `tabular-nums` (mandatory so countdown timers `01:59` never jitter horizontally).

---

## 4. Component Stylings

### 4.1 Tactile 3D Push Buttons (Primary, Secondary & Word Tiles)
- **Shape & Geometry:** Generously rounded pill-rectangles (`border-radius: 1.25rem` / `20px`) with a minimum height of `52px` for primary bottom CTAs and `46px` for interactive word tiles.
- **Elevation & Tactile Lip:** Zero blurry drop shadows or neon outer glows. Instead, every interactive button and word tile sits on a solid `4px` bottom lip:
  - *Primary CTA (`#E06D3B` fill, `#FFFFFF` text):* `border: 2px solid #B34E24; box-shadow: 0 4px 0 0 #B34E24;`
  - *Daylight Word Tile (`#FFFFFF` fill, `#18181B` text):* `border: 2px solid #E6E1D6; box-shadow: 0 4px 0 0 #D6CFC2;`
  - *Selected Word Tile (`rgba(224,109,59,0.14)` fill, `#18181B` text):* `border: 2px solid #E06D3B; box-shadow: 0 4px 0 0 #B34E24;`
  - *Dark Studio Secondary Control (`#282530` fill, `#F5F3EF` text):* `border: 1px solid rgba(255,255,255,0.12); box-shadow: 0 4px 0 0 #0D0C10;`
- **Active Interaction State:** On press (`:active`), the button translates downward `transform: translateY(3px)` and reduces its bottom lip shadow to `0 1px 0 0`, creating an unmistakable physical keycap click.

### 4.2 Collectible Phrase Cards & Sentence Jigsaw Slots
- **Phrase Card Container:** Rounded corners (`border-radius: 1.75rem` / `28px`), internal padding `24px`, `2px solid #E6E1D6` border, and a subtle warm ambient shadow (`0 10px 24px -8px rgba(24, 24, 27, 0.05)`).
- **Card Anatomy:**
  1. Top metadata row: Cultural scenario tag (`Satoshi Bold`, `12px`, uppercase) on the left + Audio speaker pill with IPA transcription (`JetBrains Mono`, `#71717A`) on the right.
  2. Center hero phrase: Target idiom rendered in `Fraunces Bold` (`28px`) with a `6px` height **Soft Apricot Wash (`rgba(224,109,59,0.22)`)** underline bar beneath the key words.
  3. Bottom context strip: Natural example sentence (`Satoshi Medium`, `15px`) and concise native meaning (`#71717A`).
- **Sentence Drop-Zone Slot:** Recessed container (`background: #F3EFE6`, `border: 2px dashed #D6CFC2`, `border-radius: 1.25rem`, `min-height: 64px`, `padding: 10px`) that snaps word tiles into alignment with a spring bounce when tapped.

### 4.3 Cozy Night AI Voice Studio Components
- **The `P` Monogram Voice Orb (Centerpiece):** A `148px × 148px` circular acoustic stage centered in the upper-middle third of the dark studio screen (`#141318`). The minimalist geometric **`P` Monogram** (left vertical pill stem + right semicircular bowl + central Ping Dot) sits at the core, surrounded by two concentric **Tangerine Pop (`#E06D3B`)** rings and a 9-bar vertical equalizer wave that scales via `transform: scaleY()` in direct response to voice input.
- **Target Phrase Mission Checklist ("The Learn-then-Speak Bridge"):** A compact container (`background: #1E1C24`, `border: 1px solid rgba(255,255,255,0.09)`, `border-radius: 1.5rem`, `padding: 16px`) docked above the microphone controls. It lists the 2–3 target phrases from Phase 1 as interactive pills:
  - *Pending State:* `background: rgba(255,255,255,0.04)`, `border: 1px dashed rgba(255,255,255,0.2)`, text in `#A1A1AA` with an empty circle icon `○`.
  - *Spoken & Verified State:* Instantly flashes into `background: rgba(224,109,59,0.20)`, `border: 1.5px solid #E06D3B`, text in `#F5F3EF`, accompanied by a floating `+50 XP` `JetBrains Mono` badge.
- **Hold-to-Speak / Hands-Free Studio Dock:** Bottom control bar featuring a central `68px` tactile 3D Tangerine Pop microphone button flanked by a `48px` "Slow Replay (`0.8x`)" button on the left and a `48px` "Hint" button on the right.

### 4.4 Header Bar & Progress Architecture
- **Top HUD Header (`height: 56px`):** Contains three clean zones with zero crowding:
  1. Left: Close/Pause icon button (`44px × 44px` tap target).
  2. Center: Chunky segmented progress bar (`height: 12px`, `border-radius: 999px`, `background: #E6E1D6` on Light / `#282530` on Dark) with a `#E06D3B` fill bar and a `3px` top highlight stripe (`rgba(255,255,255,0.35)`) for tactile volume.
  3. Right: Monospace Streak or Timer pill (`JetBrains Mono Bold`, `padding: 6px 12px`, `border-radius: 999px`).

### 4.5 Loading, Empty & Gentle Nudge States
- **Loading States:** Skeletal shimmer blocks (`border-radius: 1.5rem`) matching exact card and word-tile dimensions, sweeping a warm apricot sheen (`linear-gradient(90deg, transparent, rgba(224,109,59,0.08), transparent)`). Circular spinning loaders are strictly banned.
- **Empty States:** Composed vector graphic of the geometric **`P` Monogram** inside a dotted blueprint frame with a single-action 3D CTA button below.
- **Gentle Nudge Drawer (Feedback Sheet):** Bottom slide-up sheet (`border-radius: 2rem 2rem 0 0`, `padding: 24px`) showing the exact syllable stress in `JetBrains Mono` (`"Try: LOW-key [ˈloʊ.ki]"`) with a one-tap audio comparison button.

---

## 5. Layout Principles & Mobile Architecture

### 5.1 Viewport & Spatial Allocation (`< 768px` Mobile-First)
- **Dynamic Viewport Height:** All full-screen game and studio views must use `min-h-[100dvh]` (never `100vh` or `h-screen`) to prevent iOS Safari and Android Chrome address-bar jump bugs.
- **Safe-Area Ergonomics:**
  - Top HUD padding: `max(16px, env(safe-area-inset-top))`
  - Bottom CTA dock padding: `max(20px, env(safe-area-inset-bottom))`
  - Horizontal screen gutter: `20px` (`1.25rem`) on standard mobile (`375px–430px`).
- **Three-Zone Vertical Thumb Architecture:**
  1. **Top Zone (15% height — Scan Only):** Progress bar, streak/timer pill, and `P` Monogram badge.
  2. **Middle Stage (55% height — Cognitive Focus):** Collectible phrase card, sentence drop-zone, or the Dark Studio `P` Monogram Voice Orb + live dialogue bubble. Minimum `24px` clear vertical whitespace around the primary card.
  3. **Bottom Thumb Zone (30% height — High-Frequency Tap Area):** Interactive word bank tiles, target phrase checklist, and the full-width `52px` tactile 3D primary CTA button.

### 5.2 Grid & Anti-Overlap Discipline
- **No Overlapping Elements:** Text never overlaps monogram badges, waveform bars, or card borders. Every badge, chip, and transcript occupies its own dedicated spatial zone.
- **Asymmetric Bento Home Screen (Daily Path View):** When the user opens the app (before entering a lesson), the Home Dashboard uses an asymmetric 2-column Bento grid (`grid-template-columns: 1.35fr 1fr`, `gap: 14px`):
  - Full-width Hero Card (`span 2`): Today's 5-Minute "Learn-then-Speak" Quest with the `P` Monogram tile and primary 3D `"START SESSION"` CTA.
  - Left Wide Card (`1.35fr`): Active Phrase Vault (`Fraunces` idiom preview + mastered count).
  - Right Compact Stack (`1fr`): Two stacked monospace stat tiles (`14 DAY STREAK` and `VOICE FLUENCY 84%`).
- **Strictly Banned Layouts:** Never use 3-column equal card rows, never use `calc()` flexbox percentage hacks, and never allow horizontal overflow (`overflow-x: hidden`).

---

## 6. Motion & Interaction Philosophy

### 6.1 Spring Physics Engine
All interactive transitions use weighted spring physics—never linear or generic `ease-in-out` curves:
- **Tactile Button & Word Tile Snap:** `type: "spring", stiffness: 220, damping: 18, mass: 0.8` (crisp, responsive bounce when a word tile snaps into the sentence slot).
- **Card Stack & Sheet Transitions:** `type: "spring", stiffness: 120, damping: 20, mass: 1.0` (smooth, weighty card arrival).
- **The "Studio Shift" (Phase 1 Light → Phase 2 Dark Transition):** A `480ms` orchestrated crossfade where the background morphs from Creamy Alabaster (`#FBF9F5`) to Cozy Night Obsidian (`#141318`) while the **`P` Monogram** glides to center stage and expands its Tangerine Pop acoustic rings.

### 6.2 Perpetual Micro-Interactions
Every active screen includes one hardware-accelerated (`transform` / `opacity` only) perpetual ambient loop so the app feels alive:
- **Phase 1 (Daylight Play):** The Ping Dot inside the `P` Monogram badge performs a subtle scale pulse (`1.0 -> 1.15 -> 1.0`) every `3.2s`, and the active sentence drop-zone border pulses gently between `opacity: 0.6` and `1.0`.
- **Phase 2 (Cozy Night Voice Studio):** The 9 vertical waveform bars inside the Tangerine Pop Voice Orb run a continuous idle breathing wave (`scaleY(0.35)` to `scaleY(0.65)`) while listening, surging to `scaleY(1.25)` when speech is detected.

### 6.3 Staggered Cascade Reveals
When mounting word bank tiles or end-of-session XP summary cards, stagger each item by `45ms` (`translateY(12px) -> translateY(0)`, `opacity: 0 -> 1`). Never pop entire lists onto the screen simultaneously.

---

## 7. Anti-Patterns (Strictly Banned AI Tells)

Any generated screen or component for **PINGO** must strictly obey these **"NEVER DO"** rules:
- **NO Cartoon Animal Mascots:** Never draw birds, owls, penguins, or cartoon faces. Use the minimalist geometric **`P` Monogram** (vertical pill stem + detached semicircular bowl + central Ping Dot) exclusively.
- **NO Emojis in UI Chrome:** Never use system Unicode emojis (`🔥`, `🎉`, `🎤`, `⭐`) inside buttons, headers, or badges. Always use custom geometric vector icons matching the Pingo construction grid.
- **NO `Inter` or Generic System Fonts:** Never fall back to `Inter`, `Roboto`, `Arial`, or `Times New Roman`.
- **NO Serif Fonts in Dashboards or Controls:** `Fraunces` is strictly restricted to target English phrases and idioms. Never use `Fraunces` on buttons, settings rows, timers, or numeric stats.
- **NO Pure Black (`#000000`):** Always use Cozy Night Obsidian (`#141318`) for dark backgrounds and Charcoal Ink (`#18181B`) for dark text.
- **NO AI Purple/Blue Neon Aesthetics:** Never use purple-to-cyan gradients, glowing neon drop shadows, or sci-fi cyberpunk HUD frames.
- **NO Multi-Color Rainbow Gamification:** Do not mix random blue, purple, pink, and yellow cards on the same screen. Rely on the disciplined **Creamy Alabaster + Charcoal Ink + Tangerine Pop (`#E06D3B`)** palette.
- **NO 3-Column Equal Feature Grids:** Always use single-column mobile stacks or asymmetric 2-column Bento splits (`1.35fr / 1fr`).
- **NO Circular Loading Spinners:** Use layout-matched skeletal shimmer blocks only.
- **NO Punitive Error States:** Never flash the screen bright red or shake the entire viewport on a wrong answer; use the warm **Honey Nudge (`#D4942A`)** bottom drawer.
- **NO Generic Placeholder Copy or Names:** Never use `"Lorem ipsum"`, `"John Doe"`, `"User 123"`, or round fake percentages (`"99.9%"`, `"50%"`). Use realistic Gen Z English idioms (*"spill the tea"*, *"lowkey a masterpiece"*, *"bite the bullet"*, *"touch grass"*) and realistic metrics (`"14 DAY STREAK"`, `"01:42"`, `"84% FLUENCY"`).

---

## 8. Ready-to-Use Google Stitch Screen Prompts

Copy and paste these semantic prompts directly into **Google Stitch** alongside this `DESIGN.md` to generate cohesive mobile screens:

### Screen Prompt 1: Home Bento Quest Dashboard (Daylight Mode)
> Generate a mobile iOS screen (`390x844`) for **PINGO** following `DESIGN.md`. Use the **Creamy Alabaster (`#FBF9F5`)** background surface. At the top, place a compact header with the minimalist geometric **`P` Monogram** badge (vertical pill stem + semicircular loop with a central dot on a `#E06D3B` 3D tile) on the left and a pill badge on the right in `JetBrains Mono Bold` reading `"14 DAY STREAK"`. Below, create an asymmetric 2-column Bento grid (`1.35fr` left, `1fr` right, `14px` gap):
> 1. Full-width Hero Quest Card (`#FFFFFF` surface, `28px` radius, `2px solid #E6E1D6` border): Shows `"TODAY'S 5-MIN LOOP"` in `Satoshi Bold` (`12px`, `#71717A`), headline `"Campus Coffee & Small Talk"` in `Satoshi Black` (`22px`, `#18181B`), three interlocking phrase preview chips in `Fraunces Bold Italic` (`"my treat"`, `"rain check"`, `"catch up"`), and a full-width tactile 3D button in **Tangerine Pop (`#E06D3B`)** with a `4px` bottom lip (`#B34E24`) reading `"START PHRASE CATCH →"`.
> 2. Left Bento Card (`1.35fr`, `#FFFFFF`): `"PHRASE VAULT"` showing `"42 idioms mastered"` in `JetBrains Mono` and a featured quote card.
> 3. Right Stacked Bento Cards (`1fr`): Top card on **Cozy Night Obsidian (`#141318`)** previewing `"2:00 AI VOICE STUDIO"` with a Tangerine waveform icon; bottom card on `#FFFFFF` showing `"REFLEX SCORE: 86%"` in `JetBrains Mono Bold`.

### Screen Prompt 2: Phase 1 — Sentence Jigsaw Mini-Game (Daylight Mode)
> Generate a mobile iOS screen (`390x844`) for **PINGO Phase 1 (Phrase Catch Mini-Game)** on a **Creamy Alabaster (`#FBF9F5`)** canvas.
> - **Top HUD:** Close button on the left, chunky `12px` progress bar at `75%` filled in **Tangerine Pop (`#E06D3B`)**, and a `JetBrains Mono Bold` pill on the right reading `"COMBO 4x"` in `#E06D3B`.
> - **Prompt Card:** A Pure Cloud (`#FFFFFF`) card with a small **`P` Monogram** corner tag reading: `"When your friend's indie film turns out way better than expected, you say:"` in `Satoshi Bold` (`18px`, `#18181B`).
> - **Sentence Drop-Zone:** A recessed slot (`#F3EFE6`, `2px dashed #D6CFC2`, `20px` radius) containing `"That short film was"` (`Satoshi Bold`) followed by an active snapped tile reading `"lowkey a masterpiece"` set in `Fraunces Bold Italic` (`18px`) with a Soft Apricot fill (`rgba(224,109,59,0.14)`), `#E06D3B` border, and `/ˈloʊ.ki/` in `JetBrains Mono`.
> - **Word Bank & Bottom Dock:** Three tactile 3D white word tiles (`#FFFFFF`, `4px` bottom lip `#D6CFC2`) reading `"out of pocket"`, `"worth the hype"`, `"spill the tea"`, and a full-width bottom 3D CTA button in **Tangerine Pop (`#E06D3B`)** with `#B34E24` bottom lip reading `"LOCK IN & ENTER VOICE STUDIO →"`.

### Screen Prompt 3: Phase 2 — 2-Minute AI Voice Reflex Studio (Cozy Night Mode)
> Generate a mobile iOS screen (`390x844`) for **PINGO Phase 2 (AI Voice Reflex Studio)** on a **Cozy Night Obsidian (`#141318`)** background (strictly no `#000000`).
> - **Top Studio Bar:** Minimal back button, `"STUDIO LIVE • ROLEPLAY"` label in `JetBrains Mono` (`#A1A1AA`), and a high-contrast countdown timer pill reading `"01:38"` in `JetBrains Mono Bold` (`#F5F3EF`) with a pulsing `#E06D3B` dot.
> - **AI Dialogue Card:** Elevated **Plum Slate (`#1E1C24`)** container (`24px` radius, `1px solid rgba(255,255,255,0.09)`) with persona tag `"MAYA • FILM CLUB FRIEND"` and spoken prompt in `Satoshi Bold` (`18px`, `#F5F3EF`): `"No way you stayed up till 2 AM watching our student film! Give me your honest take—how was it?"`
> - **Centerpiece Voice Stage:** A `148px` circular **PINGO Voice Orb** featuring the minimalist geometric **`P` Monogram** surrounded by concentric **Tangerine Pop (`#E06D3B`)** acoustic rings and a 9-bar reactive vertical equalizer wave.
> - **Target Phrase Checklist ("Use in your reply"):** A `#1E1C24` mission strip showing two phrase pills set in `Fraunces SemiBold Italic`:
>   1. Checked pill (`rgba(224,109,59,0.20)` fill, `#E06D3B` border): `"✓ lowkey a masterpiece"` with a `" +50 XP "` badge in `JetBrains Mono`.
>   2. Pending pill (`rgba(255,255,255,0.04)` fill): `"○ worth the hype"`.
> - **Bottom Studio Dock:** Central tactile 3D **Tangerine Pop (`#E06D3B`)** button (`#B34E24` lip) reading `"LISTENING... TAP TO SEND REPLY"`, flanked by a `48px` `"0.8x SLOW"` button and a `48px` `"HINT"` button on `#282530`.
