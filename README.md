# Valvekliinik 10Y — Landing Page Assets

## Design Note
Single-scroll layout, white/off-white background, dark navy or forest green as accent. Typography should feel clinical-but-warm: readable sans-serif body, slightly bolder heading weight. No stock-photo-heavy feel — use real clinic photography if available.

## Files
- `copy.md` — Full Estonian copy, structured by section. No HTML. Ready for handoff to developer or Lovable.

### 2026-04-05 — Emotional clarity pass (Lasagne subagent, benchmarked against elanclinic.ee/et.html)

**Goal:** Reduce brochure feel. Strengthen calm authority. Surface the core message "you are safe here." No structural changes — surgical copy rewrites only.

**What changed:**
- **Hero sub:** Reframed from logistics-first ("2016. aastal otsustasime...") to patient-first ("Haigestuda on piisavalt raske..."). Safety cue embedded.
- **Philosophy body:** First paragraph rewritten from "Tallinna tervishoius on lünk" (consulting-brief tone) to patient-centered framing about unnecessary burden.
- **Phil-point 3:** "Edasisuunamine samas hoones" renamed to "Järgmine samm on korraldatud" — less functional, more reassuring.
- **Services h2:** "Mis juhtub, kui Valvekliinikusse tuled?" → "Kõik vajalik on koos" — calmer, more confident.
- **Floor story sub:** Added "Oled õiges kohas." — the core safety message, placed exactly where the patient is being shown the floor.
- **Journey step 1:** Added "Tule, siin on koht, kuhu tulla." — calm open invitation.
- **Journey step 5:** Tightened to "Kogu pilt on selge." — authority, not brochure.
- **Milestone statement + body:** Tightened. "Tegime lihtsa otsuse" → "asusime täitma lünka, mis ei oleks pidanud olema." More grounded. Body trimmed.
- **Footer CTA sub:** Added "Siin on koht, kuhu tulla." — closes the page on the core message.

**copy.md updated** to match all changes exactly.

**What was NOT changed:** CSS, layout, structure, FAQ, referral section, schema, nav, trust strip numbers.

---

## Chunk Log

### Chunk 1 — 2026-04-05
Hero subtitle, opening narrative (AVAJUTUSTUS, new section), trust section (USALDUSE RAAMISTIK), and service-intro (TEENUSTE ÜLEVAADE intro paragraph) fully rewritten. Goal: premium, emotionally grounded, credible. No em dashes. No discount language. Lower sections untouched.

## Changelog

### 2026-04-05 — Design and layout overhaul (senior landing-page pass)
- **Font**: switched body/heading stack to Inter (Google Fonts) for a cleaner, more premium feel
- **Color system**: refined palette; navy `#0d2d4f` as primary dark, forest green `#2a7a4e` as CTA accent (matching README guidance), removed washed-out light-blue primary CTAs
- **Hero**: added subtle CSS grid overlay texture, gradient text treatment on h1, larger font weight (800), more breathing room
- **Trust strip**: redesigned as a bordered grid (4 columns) instead of flex wrapping; better visual weight and mobile stacking
- **Added "Why Valvekliinik" 3-pillar section**: populated from copy.md trust-framework block; card top-border accent, new `#pillars` section between trust strip and services
- **Services**: filled all 5 real service cards from copy.md (previously all `[PLACEHOLDER]`); improved flex-column card layout for consistent CTA alignment at bottom
- **Ecosystem/same-floor section**: redesigned as dark navy with radial glow; service names and descriptions filled from copy.md; combined icon+heading in a flex row
- **Anniversary offer**: replaced CTA button with functional email-capture form (styled inline, green palette); JS `handleOfferForm` placeholder handler included
- **Referral**: added `share-box` with actual share text from copy.md; copy-to-clipboard button with clipboard API + execCommand fallback; JS `copyShareText` function
- **FAQ**: all 6 questions and answers filled from copy.md (previously all `[PLACEHOLDER]`); chevron redesigned as circular badge
- **Header**: backdrop-filter blur on sticky nav; green nav-cta button
- **Footer CTA**: dark navy gradient; used actual "Kümmend aastat hiljem, ikkagi sinu kõrval." headline from copy.md
- **Footer**: filled address (Lõõtsa 2, Ülemiste Tervisemaja, Tallinn), founding year 2016, actual services list; footer wordmark at 800 weight
- **Schema.org**: added JSON-LD `MedicalClinic` markup in head
- **Accessibility**: `role="region"` on FAQ answers, `aria-label` on email input, `focus-visible` outlines on all links
- **Mobile**: improved grid stacking breakpoints, larger touch targets, reduced card padding on small screens
- **No em dashes used anywhere. No fake claims. All remaining `[PLACEHOLDER]` values explicitly marked for clinic to fill (phone, email, hours, social links).**

### 2026-04-05 — Copy review and rewrite (senior conversion copy pass)
- **Hero headline** rewritten: "10 aastat. Üks koht. Kogu vastus." → "Kümme aastat. Iga kord kohal, kui loeb." (specific, emotionally resonant, ties urgency to anniversary)
- **Hero subtitle** rewritten to lead with founding intent rather than generic gratitude; removed "Täname iga patsienti" framing
- **Trust section headline** changed from defensive "Miks Valvekliinik?" to assertive "Kümme aastat ei ole lihtsalt number."
- **Trust section body** rewritten: from feature list to earned-credibility narrative
- **Pillar 2 label** changed from "Lühike ooteaeg" to "Samal päeval" (outcome-first language)
- **Services intro** tightened; removed filler phrase "midagi enamat kui kliinik"
- **Anniversary section** fully reframed: "Juubelipakkumine" → "Juubeliaasta algatus"; explicitly states "Mitte hinnasoodustust" to avoid cheap discount perception; removed reference to "pikaajalised patsiendid"
- **Referral headline** changed from question ("Tunned kedagi...?") to assertion ("Hea arst on väärt jagamist.")
- **Referral body** tightened; sharing text made more natural
- **Bottom CTA body** changed from unsubstantiated "tuhandeid tallinnlasi valib just Valvekliiniku" to honest "tule veendu ise, millest räägime"
- **FAQ** minor polish throughout; removed assumption about free parking
- No em dashes used anywhere. No cheap discount language. No prior patient history references.

### 2026-04-05 — Material rebuild (quality uplift pass, Lasagne subagent)

**What was materially rebuilt (not polished):**

- **Hero**: Completely rewritten. Old headline ("10 aastat. Üks koht. Kogu vastus.") replaced with a two-line editorial structure: "Alati kohal. / Kümme aastat järjest." Badge redesigned — party emoji removed, replaced with a subtle green-dot live indicator + year range. Subtitle now leads with a specific founding intent and names the address (Sepapaja 12/1, 3rd floor) to feel grounded. Secondary CTA is now the phone number itself, not a vague "Vaata teenuseid".

- **Philosophy section (new)**: Replaced the 3-pillar card grid with an editorial two-column layout. Left column carries a strong statement ("Arstiabi ei peaks olema logistikaülesanne.") plus a narrative that positions Valvekliinik in the real healthcare gap. Right column has 3 bordered points with icon tiles — feels like editorial callouts, not feature cards.

- **Floor Story section (new)**: Completely replaced the old ecosystem card grid (6 equal navy cards) with a patient journey visualization — 5 numbered steps with a connecting vertical line. Tells the actual experience of arriving at the 3rd floor as a story: arrival, doctor, lab, specialist, departure with solution. This makes "same floor" feel like a clinical advantage, not a list of tenants.

- **Milestone / Anniversary section (rebuilt)**: The old "offer" section (green gradient, email capture form, "Kümne aasta tänuks") was stripped. The new section uses a large watermark "10" behind editorial text, a gradient divider bar, and a centered two-CTA group (book + email). The email capture is preserved but repositioned as a secondary element below the primary CTAs. No cheap discount language. No "offer" framing.

- **All placeholder contact data filled in**: Every `[TELEFON]` replaced with `+372 5 911 0909`. Every `[EPOST]` replaced with `info@valvekliinik.ee`. Old footer had duplicate contact lines — cleaned up.

- **Address corrected throughout**: copy.md previously had "Lõõtsa 2" in the FAQ and footer section. Now correctly Sepapaja 12/1, 3. korrus throughout all files.

- **Terminology corrected**: "kiirabiasutus" in the sharing text replaced with "erakorralise meditsiini kliinik". No "kiirabi" usage anywhere. Consistent throughout both files.

- **Footer CTA rewritten**: From "Kümmend aastat hiljem, ikkagi sinu kõrval." (sentimental, vague) to "Vastuvõtt on saadaval. Täna ka." (confident, direct, action-forward).

- **Hero gradient refined**: Darker, deeper navy gradient (4-stop) instead of the lighter 3-stop. Dot grid texture replaced with subtle radial dot pattern. Soft bottom glow added for depth.

- **Service cards**: Top-bar accent now fades in on hover (opacity 0, transitions to 1) rather than always visible — cleaner at rest. Copy tightened throughout.

- **Nav link anchors updated** to match new section IDs (`#kolmas-korrus` for floor story, `#juubel` for anniversary).

- **Schema.org updated**: Added telephone, email, postalCode fields.

- **copy.md fully rewritten**: Now a clean structured document matching the rebuilt HTML exactly. Includes terminology rules section and SL Tervisekeskus adaptation notes.

**What was NOT changed:**
- Core CSS variable system and color palette (already solid)
- FAQ structure and questions (minor copy polish only)
- Referral/share section (fixed "kiirabiasutus" → "erakorralise meditsiini kliinik" only)
- Services card count (still 5)
- Font stack (Inter)
- Schema.org base structure

## Reuse Notes for SL Tervisekeskus Adaptation
- Replace "Valvekliinik" with "SL Tervisekeskus" and update founding year + anniversary context accordingly.
- The same-floor ecosystem section maps well to SL Tervisekeskus's multi-specialty model; swap in SL-specific services and any unique differentiators (e.g. continuity of care, founding family history).
- Remove urgent-care-specific language (infusioonravi, haavahooldus) unless those services also apply; replace with SL's primary care and preventive health framing.
- CTA and FAQ structure can be reused as-is with minor text swaps.
- Anniversary offer placeholder section is optional for SL — can be repurposed as a seasonal campaign block instead.

### 2026-04-05 — Chunk 2: Top-half visual structure rebuild
- **Top bar**: Added a slim announcement ribbon above the nav ("2016-2026 | Kümme aastat Tallinnas") in dark navy.
- **Hero**: Replaced centered brochure layout with an editorial split layout (left: headline + body + CTAs, right: circular "10" year mark + 3 stat chips). New `.hero-kicker`, `.hero-headline`, `.hero-body`, `.hero-actions` classes. Stronger type hierarchy, left-aligned on desktop, stacked on mobile.
- **Trust strip + Pillars**: Removed both. Replaced with a single `.narrative` section: left side is an editorial origin-story with heading + 2 paragraphs; right side is a clean bordered `.narrative-proof` block with 4 key stats (10y, 5+ specialties, 7 days, <24h). Reads as earned authority rather than feature checklist.
- **Services intro**: Replaced generic `.section-header` with a responsive `.services-head-row` (heading left, lead copy right on desktop). Cleaner editorial transition into the service grid.
- **CSS cleanup**: Removed orphaned CSS for `.hero-badge`, `.hero-sub`, `.hero-buttons`, `.trust-strip`, `.pillars`, and related rules.
- No em dashes used anywhere in this chunk.
