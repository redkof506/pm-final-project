# Experimentation Plan

> Module 5 · Run Effective Product Experimentation — ★ Deliverable 5

## Overview

A/B test on StreamLine (B2C) validating whether a Mood-Based Entry Point — letting users pick a mood on login to filter the rail — reduces choice friction for "The Overwhelmed Browser" persona before full-scale development. Control (A) is the standard entry screen with no mood-based recommendation; Variant (B) surfaces mood chips on entry that filter the rail to the selected mood. Everything else — including the skip path, which returns users to the standard screen unchanged — is held constant between arms. Success is measured on Homepage Visit → Start Playing conversion (baseline 29%, MDE 5%, 1,354 users/arm, 50/50 split, α = 0.05), over an 8-week fixed read window, while protecting Power User segment performance as a guardrail.

_____

## What you're testing

| Element | Detail |
|---|---|
| Hypothesis under test | I believe that Mood-Based Entry Point — Pick a mood on login to filter the rail — for "The Overwhelmed Browser" (a casual-but-invested viewer sitting down for a specific mood, e.g. "quiet Sunday night," rather than a specific title) will result in reducing the friction point of user choice, allowing an increase in Conversion funnel (30+ sessions) and subscription retention cohort heatmap, as measured by a 5% change in Engagement & Funnel Health (last 90 days) — Homepage Visit → Start Playing — within 8 weeks (2 weekly cycles). We will protect User Segment Performance for Power users, which must not drop, throughout the test. |
| Experiment design (A/B, etc.) | A/B test, 50/50 traffic split, 1,354 users per arm, 8-week fixed duration (2 weekly cycles), significance threshold p < 0.05.<br>**Control (A):** Standard application entry with past films, new entries, and no recommendation option based on current mood.<br>**Variant (B):** Mood chips visible on the entry screen; selecting a chip filters the rail to that mood.<br>**Held constant (isolation check):** If a user chooses to skip, no changes to the app — they return to the standard screen with past films, new entries, and no mood-based recommendation, identical in both arms. |
| Primary metric | Engagement & Funnel Health (last 90 days) — Homepage Visit → Start Playing. Baseline rate: 29%. Minimum Detectable Effect: 5%. |
| Guardrail metric | User Segment Performance for Power users — must not drop. Guardrail boundary: 0.5 pts. |
| Decision rule (ship / kill / pivot) | **Ship** if Homepage Visit → Start Playing improves by ≥ 5% at p < 0.05 and Power User segment performance does not drop by 0.5 pts. or more, after 8 weeks (2 weekly cycles).<br>**Iterate** if direction is positive but lift is below the MDE.<br>**Kill** if the primary metric shows no improvement or moves negatively.<br>Read date is fixed at the end of 8 weeks (2 weekly cycles) — no results reviewed before this date. |

## Findings & decision _(after running it)_

_[To be completed once the test has run.]_
