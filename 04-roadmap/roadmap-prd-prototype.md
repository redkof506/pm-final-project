# Roadmap, PRD & Prototype — StreamLine Spotlight

> Module 4 · Build High-Velocity Product Roadmaps — ★ Deliverable 4

**Team:** 2 engineers + 1 designer

## High-level product roadmap

**Strategic anchors**
- **Persona:** "The Overwhelmed Browser" — a casual-but-invested viewer sitting down for a specific mood (e.g., "quiet Sunday night") rather than a specific title.
- **Primary metric:** Engagement & Funnel Health (last 90 days) — 30+ min sessions — target increase of 10+%.
- **Moment of misery:** There's no mood- or context-based browsing pathway — discovery is structured entirely around recency/genre rows, and natural-language search doesn't work reliably (only exact titles do). The volume of choice itself becomes the enemy: this is the user who eventually gives up trying anything new and defaults to rewatching a small known set — quiet disengagement, not a complaint ticket.
- **Guardrail:** User Segment Performance for Power users must not drop.

**Feature scoring (Value / Effort / Quadrant / Decision)**

| Feature | Value | Effort | Quadrant | Decision | Rationale |
|---|---|---|---|---|---|
| A1 Spotlight Curated Rail | 5 | 2 | Quick Win | Now | Directly replaces the failed recency/genre discovery model with a human-curated escape hatch — ships fast since it's placement + editorial ops, not new infra. |
| A2 "Why You'll Love This" Label | 4 | 3 | Major Project | Next | Attacks decision paralysis at the exact moment it happens, but generating trustworthy per-title reasoning at scale is real model/copy work, not a UI tweak. |
| A3 Hidden Gem Badge | 2 | 1 | Fill-In | Later | Cheap to ship but a badge doesn't solve "I don't know where to start for my mood" — it's decoration on rows the persona already ignores. |
| A4 Mood-Based Entry Point | 5 | 4 | Major Project | Now | This is the moment of misery, named directly — but it requires mood-tagging the catalog and new onboarding logic, which is months not days even at MVP scope. |
| A5 Personalized Spotlight Queue | 3 | 4 | Time Sinker | Later | Taste-profile AI is just the existing algorithm wearing a new name — the persona's problem isn't lack of personalization, it's lack of a mood/context lens, so high build cost buys little incremental value. The main work would be a full rework of the algorithms, which usually takes weeks of work and tests alone. |
| A6 Spotlight Digest Email | 2 | 2 | Fill-In | Later | Nice retention nudge but it's off-platform and doesn't touch the in-session browsing failure that's actually driving quiet disengagement. |
| A7 Curator Profiles | 3 | 4 | Time Sinker | Cut | Follow-a-curator is a good long-term discovery layer, but building profiles + follow graph + editorial pipeline in 8 weeks is disproportionate to what it buys this persona right now. |
| A8 Watch Party (Spotlight) | 1 | 5 | Time Sinker | Cut | Solves a social-viewing problem the Overwhelmed Browser doesn't have — this is Sales chasing a use case orthogonal to the discovery failure; kill it for this initiative. |
| A9 Advanced Filter Engine | 2 | 3 | Time Sinker | Cut | More filters is more choice, which is the disease, not the cure — it hands the overwhelmed persona another decision tree instead of removing one. |
| A10 Offline Download (Spotlight) | 1 | 4 | Time Sinker | Cut | Doesn't address discovery at all and doesn't move 30+min session engagement — another Sales ask riding on the Spotlight name with no anchor connection. |

**Phased execution**

- **NOW — 3-week sprint**
  - **A1 Spotlight Curated Rail** — directly replaces the failed recency/genre discovery model with a human-curated escape hatch; ships fast since it's placement + editorial ops, not new infra.
  - **A4 Mood-Based Entry Point** — this is the moment of misery, named directly, but requires mood-tagging the catalog and new onboarding logic, which is months not days even at MVP scope.

- **NEXT — following 1–2 sprints**
  - **A2 "Why You'll Love This" Label** — attacks decision paralysis at the exact moment it happens, but generating trustworthy per-title reasoning at scale is real model/copy work, not a UI tweak.

- **LATER — backlog**
  - **A3 Hidden Gem Badge** — cheap to ship but doesn't solve "I don't know where to start for my mood."
  - **A5 Personalized Spotlight Queue** — taste-profile AI wearing a new name; the persona's problem is lack of a mood/context lens, not lack of personalization.
  - **A6 Spotlight Digest Email** — nice retention nudge but off-platform, doesn't touch the in-session browsing failure driving disengagement.

- **✂ Cut List**
  - **A7 Curator Profiles** — good long-term discovery layer, but disproportionate build cost for what it buys this persona right now.
  - **A8 Watch Party (Spotlight)** — solves a social-viewing problem the Overwhelmed Browser doesn't have; orthogonal to the discovery failure.
  - **A9 Advanced Filter Engine** — more filters is more choice, which is the disease, not the cure.
  - **A10 Offline Download (Spotlight)** — doesn't address discovery at all and doesn't move 30+min session engagement.

_____

## PRD snippets

**Feature scoped ("Now"):** Mood-Based Entry Point — Pick a mood on login to filter the rail.

**Finalized Must-Haves (after overriding the AI):**
1. **Fixed mood selector (closed set of chips), non-blocking placement** — surfaced at login/home but never a full-screen forced gate. A mandatory modal is the single fastest way to violate the Power User guardrail: they already know what they want, and forcing a detour before every session is a direct tax on their 4.8×/week habit.
2. **One-tap skip/bypass to standard browse** — must be at least as fast as ignoring the feature entirely. This is what protects the guardrail structurally, not just by policy.
3. **Rail actually filters on mood selection** — the core mechanic; without it there's nothing to measure.
4. **Minimum viable editorial mood-tagging** — enough curated titles per mood that a selection doesn't dead-end into thin or repetitive results, which would suppress session length rather than grow it.
5. **Session-length instrumentation attributed to entry path** — every session must be tagged by whether it originated from a mood selection, with duration tracked against the 30-minute threshold. Without this, the Primary Metric cannot be reported at all — this isn't a nice-to-have, it's the difference between shipping a feature and shipping an unmeasured guess.

**Demoted from Must → Should/Won't:**
- **Segment tagging on every event (Power / Casual / Wanderer)** — not a dashboard, just the underlying data field. Originally considered a Day-1 must-have since the guardrail requires knowing from day one whether Power User behavior moved; waiting until a later sprint would mean shipping without the ability to detect a guardrail breach in real time. Ultimately fully removed, since user type and feature-usage initiation can already be defined without it.

**What the PRD makes explicit that a vague brief would have missed:** The importance of the feature not encroaching on the app's existing core features, and ensuring fast, frictionless transition back to standard search/browse.

_____

## Wireframes / prototype

**Prototype gap check:** The prototype largely confirmed the PRD logic — it solves the core moment of misery by allowing users to filter the available film set using mood-based choices, with easy access, fast return, and easy cancellation/skip back to standard browse.

**Prototype:** https://lovable.dev/preview/l7ZzBqumJYewAz6HfAjjprGroM4ptSkZ

**Roadmap artifact:** spotlight-roadmap.html — interactive HTML roadmap visualizing the NOW/NEXT/LATER lanes and Cut List above.
