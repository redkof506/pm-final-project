# Feature Roadmap, Module 4 · StreamLine Spotlight

**Team:** 2 engineers + 1 designer

## Strategic anchors
- **Persona:** "The Overwhelmed Browser" A casual-but-invested viewer sitting down for a specific mood (e.g., "quiet Sunday night") rather than a specific title.
- **Primary metric:** Engagement & Funnel Health (last 90 days) - 30+ min sessions - increased 10+%
- **Moment of misery:** There's no mood- or context-based browsing pathway — discovery is structured entirely around recency/genre rows, and natural-language search doesn't work reliably (only exact titles do). The volume of choice itself becomes the enemy: this is the user who eventually gives up trying anything new and defaults to rewatching a small known set — quiet disengagement, not a complaint ticket.
- **Guardrail:** User Segment Performance for Power users must not drop

## Scoring
| Feature | Value | Effort | Quadrant | Decision | Rationale |
|---|---|---|---|---|---|
| A1 Spotlight Curated Rail | 5 | 2 | Quick Win | Now | Directly replaces the failed recency/genre discovery model with a human-curated escape hatch — ships fast since it's placement + editorial ops, not new infra. |
| A2 'Why You'll Love This' Label | 4 | 3 | Major Project | Next | Attacks decision paralysis at the exact moment it happens, but generating trustworthy per-title reasoning at scale is real model/copy work, not a UI tweak. |
| A3 Hidden Gem Badge | 2 | 1 | Fill-In | Later | Cheap to ship but a badge doesn't solve "I don't know where to start for my mood" — it's decoration on rows the persona already ignores. |
| A4 Mood-Based Entry Point | 5 | 4 | Major Project | Now | This is the moment of misery, named directly — but it requires mood-tagging the catalog and new onboarding logic, which is months not days even at MVP scope. |
| A5 Personalized Spotlight Queue | 3 | 4 | Time Sinker | Later | Taste-profile AI is just the existing algorithm wearing a new name — the persona's problem isn't lack of personalization, it's lack of a mood/context lens, so high build cost buys little incremental value. The main work would be in the full rework of the algorithms which usually takes weeks of work and tests only. |
| A6 Spotlight Digest Email | 2 | 2 | Fill-In | Later | Nice retention nudge but it's off-platform and doesn't touch the in-session browsing failure that's actually driving quiet disengagement. |
| A7 Curator Profiles | 3 | 4 | Time Sinker | Cut | Follow-a-curator is a good long-term discovery layer, but building profiles + follow graph + editorial pipeline in 8 weeks is disproportionate to what it buys this persona right now. |
| A8 Watch Party (Spotlight) | 1 | 5 | Time Sinker | Cut | Solves a social-viewing problem the Overwhelmed Browser doesn't have — this is Sales chasing a use case orthogonal to the discovery failure; kill it for this initiative. |
| A9 Advanced Filter Engine | 2 | 3 | Time Sinker | Cut | More filters is more choice, which is the disease, not the cure — it hands the overwhelmed persona another decision tree instead of removing one. |
| A10 Offline Download (Spotlight) | 1 | 4 | Time Sinker | Cut | Doesn't address discovery at all and doesn't move 30+min session engagement — another Sales ask riding on the Spotlight name with no anchor connection. |

## Roadmap
### NOW, 3-week sprint
- **A1 Spotlight Curated Rail**, Directly replaces the failed recency/genre discovery model with a human-curated escape hatch — ships fast since it's placement + editorial ops, not new infra.
- **A4 Mood-Based Entry Point**, This is the moment of misery, named directly — but it requires mood-tagging the catalog and new onboarding logic, which is months not days even at MVP scope.

### NEXT, following 1-2 sprints
- **A2 'Why You'll Love This' Label**, Attacks decision paralysis at the exact moment it happens, but generating trustworthy per-title reasoning at scale is real model/copy work, not a UI tweak.

### LATER, backlog
- **A3 Hidden Gem Badge**, Cheap to ship but a badge doesn't solve "I don't know where to start for my mood" — it's decoration on rows the persona already ignores.
- **A5 Personalized Spotlight Queue**, Taste-profile AI is just the existing algorithm wearing a new name — the persona's problem isn't lack of personalization, it's lack of a mood/context lens, so high build cost buys little incremental value. The main work would be in the full rework of the algorithms which usually takes weeks of work and tests only.
- **A6 Spotlight Digest Email**, Nice retention nudge but it's off-platform and doesn't touch the in-session browsing failure that's actually driving quiet disengagement.

### ✂ Cut List
- **A7 Curator Profiles**, Follow-a-curator is a good long-term discovery layer, but building profiles + follow graph + editorial pipeline in 8 weeks is disproportionate to what it buys this persona right now.
- **A8 Watch Party (Spotlight)**, Solves a social-viewing problem the Overwhelmed Browser doesn't have — this is Sales chasing a use case orthogonal to the discovery failure; kill it for this initiative.
- **A9 Advanced Filter Engine**, More filters is more choice, which is the disease, not the cure — it hands the overwhelmed persona another decision tree instead of removing one.
- **A10 Offline Download (Spotlight)**, Doesn't address discovery at all and doesn't move 30+min session engagement — another Sales ask riding on the Spotlight name with no anchor connection.
