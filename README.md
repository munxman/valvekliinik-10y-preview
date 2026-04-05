# Valvekliinik 10Y — Landing Page Assets

## Design Note
Single-scroll layout, white/off-white background, dark navy or forest green as accent. Typography should feel clinical-but-warm: readable sans-serif body, slightly bolder heading weight. No stock-photo-heavy feel — use real clinic photography if available.

## Files
- `copy.md` — Full Estonian copy, structured by section. No HTML. Ready for handoff to developer or Lovable.

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

## Reuse Notes for SL Tervisekeskus Adaptation
- Replace "Valvekliinik" with "SL Tervisekeskus" and update founding year + anniversary context accordingly.
- The same-floor ecosystem section maps well to SL Tervisekeskus's multi-specialty model; swap in SL-specific services and any unique differentiators (e.g. continuity of care, founding family history).
- Remove urgent-care-specific language (infusioonravi, haavahooldus) unless those services also apply; replace with SL's primary care and preventive health framing.
- CTA and FAQ structure can be reused as-is with minor text swaps.
- Anniversary offer placeholder section is optional for SL — can be repurposed as a seasonal campaign block instead.
