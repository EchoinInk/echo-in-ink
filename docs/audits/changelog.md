# Changelog

## 2026-06-24 — Audit Notes and Repo Docs

This week’s highlights:

- Added a refreshed README with the current project stack, local development, build, and contact-form notes.
- Produced a new design inconsistencies report to capture source-verified review risks and intentional exceptions.
- Reworked the design system audit and added a concise audit-priorities brief for future reviews.

## 2026-06-21 — Lumo and Homepage Polish

This week’s highlights:

- Updated the Lumo case study with cinematic production polish and a long-form numbered story structure.
- Refined the Home page with clearer proof hierarchy, an early proof strip, and stronger service-card distinction.
- Updated the Works page with tighter proof sequencing, an editorial testimonial, and a calmer closing CTA.
- Updated the Studio page with unified section rails and aligned editorial section structures.

## 2026-06-19 — Orbitals and Repo Cleanup

This week’s highlights:

- Added a new visual Orbitals page and expanded the orbitals set to 30 total entries.
- Standardised page rails and the typography system across the main page set.
- Simplified shared page hero variants and tightened hero CSS overrides.
- Removed unused scaffolds, pruned archive leftovers, and cleaned related styling files.
- Ran a formatting sweep across core token and typography files.

## 2026-06-09 — Redesigned Page Registry

Current active redesigned pages:

- `/` — `HomePage`
- `/identity` — `IdentityPage`
- `/sessions` — `SessionsPage`
- `/worlds` — `WorldsPage`
- `/works` — `WorksPage`
- `/works/lumo` — `LumoPage`
- `/studio` — `StudioPage`
- `/contact` — `ContactPage`
- `/systems` — `SystemsPage`
- `/archive` — `ArchivePage`

Maintenance notes:

- Active route source of truth: `src/App.tsx`.
- Page modules now use named exports.
- `EasyPage.tsx` not routed.
- Archive folders excluded unless imported.

---

## 2026-06-08 — WCAG Contrast and Focus Pass

- Improved muted text contrast.
- Strengthened visible focus indicators.
- Improved form labels, placeholders, footer links, subtle-link readability.
- Fixed system status pill contrast.
- Refined mobile navigation Close button focus ring.

---

## 2026-06-04 — Design System Migration: Echo in Ink Palette Update

### Color Token System Migration

#### Core Palette Update

- Migrated Aurora/Luxe/Orchid → Echo in Ink.
- New core tokens: `--ei-void`, `--ei-ink`, `--ei-midnight`.
- New accent tokens: `--ei-electric-blue`, `--ei-halo-blue`, `--ei-violet`, `--ei-echo-magenta`, `--ei-soft-neon`.
- New typography colors: `--ei-moonlit`, `--ei-ice-white`.

#### Deprecated Aliases

- Backward-compatibility aliases added.
- All deprecated RGB variants mapped.

#### Semantic Tokens

- Added text, component, gradient, glow, shadow, and ring tokens.
- New: `--ei-button-focus-ring`.

### Typography System Consolidation

- Unified `typography.css` + `typography-enhanced.css` → `typography-system.css`.
- Added full font-face declarations.
- New canonical naming: `.ei-type-*`.
- Legacy classes aliased.

### CSS Architecture Cleanup

- Reorganized `globals.css` import order.
- Removed deprecated imports.
- Consolidated atmospheric files.

### Component Updates

- Updated 40+ components to new tokens.
- Updated gradients, glows, and inline color values.

### Quality Assurance

- Build passed.
- Linter passed.
- CSS bundle reduced.
- No breaking changes.

---

## 2026-06-01 — Studio Page Redesign

### New Components

- `StudioHero`
- `NumberedSectionLabel`
- `EyebrowLabel`
- `OriginSection`
- `QuoteCard`
- `PhilosophyGrid`
- `ValuesGrid`
- `StudioCTA`
- `PhilosophyCard`
- `studioContent.ts`

### Design Notes

- Hero image uses left-edge gradient blend.
- Quote card: indigo surface, serif italic, subtle glow.
- CTA: horizon crop, text left / image right.

---

## 2026-06-01 — Works Page Redesign

### Works Page Restructure

- Rebuilt Works page with cinematic hero, filter bar, grid, and CTA.
- Removed custom footer strip.
- Updated SEO metadata.

---

## 2026-05-29 — Works Page Implementation (Phase 5)

### New Component

- `EditorialHero`
- `ProjectCard`
- `WorkFilterBar`
- `WorksGrid`
- `ProjectCTA`
- `worksProjects.ts`

### WorksPage.tsx Rewrite

- Replaced inline hero with `EditorialHero`.
- Added filter bar, grid, CTA.
- Updated SEO.
- Removed legacy gallery.

### Design System

- Updated card tokens, filter states, hover interactions.
- Motion via `motion-cinematic`.

### Token Cleanup

- Updated muted/soft text tokens.

### Imagery

- Wired hero, card, and CTA images.

### Verification

- TS: 0 errors.
- Vite: exit 0.

---

## 2026-05-27 — Homepage + Systems + Pathways Refinement (Phase 5)

### Pathways.tsx Rewrite

- Four transformation cards.
- OrbitalVisual icons.
- Editorial titles + mono CTAs.
- Removed legacy image cards.

### LumoCaseStudyTeaser.tsx Refactor

- 2-column layout.
- Discipline tags.
- Route fix.
- Ambient glow layer.

### EmergingSystems.tsx Rewrite

- Five system cards.
- Eyebrow + link header.
- `lg:grid-cols-5`.

### ClosingSection.tsx

- Updated description.

### Footer.tsx Rewrite

- Four-column layout.
- Updated location.
- Added OrbitalVisual.

### Home.tsx Order

- Hero → Philosophy → Pathways → Lumo → Systems → Closing → Footer.

### Build

- TS: 0 errors.
- Vite: exit 0.

### Known Outstanding

- `/systems` route missing.
- Orphaned components preserved.

---

## 2025-05-26 — Third Refinement Pass (Phases 4–7)

### Phase 4 — Card Archetype Differentiation

- Added `archetype` prop to `GlowCard`.
- Sessions / Identity / Worlds archetypes with unique glow and vignette profiles.

### Phase 5 — How We Work

- Four-phase operational anchor.
- Minimal vertical flow.
- Gradient connector line.

### Phase 6 — Footer Polish

- Simplified gradients.
- Adjusted spacing and dissolve heights.

### Phase 7 — Mobile + Performance QA

- Responsive breakpoints.
- Reduced blur.
- GPU-friendly motion.
- No parallax.

---

## 2025-05-26 — Refinement Phase

### 7-Phase Homepage Refinement

#### Phase 1 — Hero Clarity

- Added supporting positioning line.

#### Phase 2 — CTA Hierarchy

- Primary / Secondary / Tertiary button system.

#### Phase 3 — Readability Refinement

- Increased opacity across typography.

#### Phase 4 — Conversion Anchor

- Created `WhatWeCreate.tsx`.

#### Phase 5 — Tempo Change Section

- Created `CinematicStatement.tsx`.

#### Phase 6 — Card Differentiation

- Added `featured` and `glowPosition`.

#### Phase 7 — Footer Rebuild

- Cinematic conclusion with fade.

---

## 2025-05-26 — Structural Corrections

### Restored

- Homepage structure restored.

### Added

- Motion identity system.
- Atmospheric continuity.
- Hero depth separation.
- Footer epilogue.

### Corrected

- Full spacing pass.
- Reduced section spacing.
- Fixed Pathways spacing.
- Reduced AtmosphericBridge.
- Simplified gradients.
- Streamlined transitions.

### Final Structural Corrections

- Compressed all sections to `spacing="sm"`.
- Removed AtmosphericBridge.
- Adjusted ClosingSection spacing.
- Rebuilt Footer.
- Tightened gaps across all sections.
