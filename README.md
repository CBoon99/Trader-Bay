## Trader Bay — Swap / Trade / Gift (Education-First)

Single-page, front-end prototype for a trusted, family-friendly marketplace. Focus: education-first, on-platform safety, mode-aware flows (swap/trade/gift), and transparent policies.

### Quick Start
- Open `trader-bay.html` in a modern browser (Chrome/Edge/Safari/Firefox).
- Assets live in `Assets/` (logo + listing images). Keep paths if you move the HTML.

### Core Features
- **Brand & UI:** New palette, Inter/Plus Jakarta Sans, premium glass hero, responsive grid/cards with hover quick-actions (desktop) and mobile-friendly layout.
- **Mode-aware:** Swap/Trade/Gift toggles color-coded; offer modal adapts per mode (swap picker, trade points slider, gift request flow).
- **Kid/Parent gating:** Kid accounts default to quick messages only; parent-supervised toggle can enable free text; parent approval badges; parent panel for oversight.
- **Safety:** Pinned “no personal info” in messages, safety checkboxes before offers, safety guide + reporting guidance, Esc-close + focus trap in modals, prefers-reduced-motion handling.
- **Filters & chips:** Resettable filters with active chips; mode filter integrated.
- **Listings:** Real images with emoji overlays, mode gradients, delivery/type chips, consistent meta, trust stats.
- **Education & trust:** Positioning note (learn-first), ingredient/knowledge accordions, trust strips, policies deck, education placeholder, AI-support note.
- **Anchors:** Nav links to Policies, Education, Trust, Contact, Safety; smooth scroll.

### Key Paths
- `trader-bay.html` — all markup, styles, and JS (no build step).
- `Assets/` — `logo.png` and listing images:
  - `pokemon-cards.png`, `minecraft-armor.png`, `harry-potter-books.png`, `lego-falcon.png`, `roblox-items.png`, `science-kit.png`, `football-boots.png`, `vintage-gameboy.png`, `art-supplies.png`, `minecraft-blueprints.png`, plus `Site images.png` (source sheet).

### Behavior Notes
- **Modals:** aria-modal, role, Esc to close, click-off closes, basic focus trap.
- **Loading state:** Offer submit and Create Listing show spinner.
- **Responsive:** Hover quick-actions hidden on touch; mobile nav bar present; cards and grids adapt down to ~240px columns.
- **Safety guide:** Located under Policies (`#safety`) with concise meetup/digital guidance.

### How to Customize
- **Brand:** Update `:root` variables for colors/shadows; swap `Assets/logo.png`.
- **Imagery:** Replace images in `Assets/` and adjust `imageSrc` entries in the listings array.
- **Copy:** Edit positioning note, education accordions, policy cards, and safety guide text inline in `trader-bay.html`.
- **Gating logic:** See `applyAccountGating` and `renderOfferModalContent` for supervision and safety checkbox flows.

### Accessibility
- Prefers-reduced-motion honored.
- Focus trap + Esc in modals; smooth-scroll anchors.
- Color contrast set against light neutrals; buttons have hover/focus affordances.

### What’s Not Included
- No backend, auth, real messaging, payments, or persistence.
- No real moderation or reporting pipeline—UI only.
- No build tooling; everything is static.

### Next Steps (if needed)
- Wire “Contact” to a real email/form endpoint.
- Add real support chatbot/FAQ backend.
- Expand Education/Research into structured articles.
- Add telemetry/consent (analytics) if required—document in Privacy/Cookies first.

