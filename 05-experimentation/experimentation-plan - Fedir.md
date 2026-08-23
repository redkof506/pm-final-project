# Experimentation Plan (Module 5)

## Get your documents ready
- **From M3, your hypothesis sentence:** Based on the fact that only 11% of viewers reach 30+ min session, we believe that solving Tailored to the user need film choices based on this current state of mind or mood or ability to use fuzzy search with key words to find out the right recommendations for "The Overwhelmed Browser" A casual-but-invested viewer sitting down for a specific mood (e.g., "quiet Sunday night") rather than a specific title. will result in reducing the friction point of the user choice, allowing to increase 2 metrics: Conversion funnel (30+ sessions) and subscription retention cohort heatmap., as measured by Engagement & Funnel Health (last 90 days) - 30+ min sessions. We will protect User Segment Performance for Power users must not drop and make a go/no-go decision after 8 weeks.
- **From M3, your primary success metric & guardrail metric:** Engagement & Funnel Health (last 90 days) -Homepage Visit → Start Playing
- **From M4, the feature you scoped in your PRD this is what you're testing:** Mood-Based Entry Point - Pick a mood on login to filter the rail

## Define your experiment parameters
- **Feature under test pull from your M4 PRD:** Mood-Based Entry Point - Pick a mood on login to filter the rail
- **Persona pull your M2 persona:** "The Overwhelmed Browser" A casual-but-invested viewer sitting down for a specific mood (e.g., "quiet Sunday night") rather than a specific title.
- **Expected outcome the behaviour change you expect, from your M3 hypothesis:** reducing the friction point of the user choice, allowing to increase 2 metrics: Conversion funnel (30+ sessions) and subscription retention cohort heatmap.
- **Primary success metric the one number that defines success, from M3:** Engagement & Funnel Health (last 90 days) -Homepage Visit → Start Playing
- **Baseline rate today's rate of your primary metric, from your M3 data:** 29%
- **Guardrail metric & boundary what must not break, and how far it can move before you investigate:** User Segment Performance for Power users must not drop
- **Minimum Detectable Effect (MDE) the smallest improvement worth shipping, your floor:** 5%
- **Sample size per arm use the calculator in the builder, baseline + MDE:** 1354
- **Traffic split & test duration 50/50 standard · cover ≥ 2 weekly cycles:** 50/50
- **Significance threshold p < 0.05 is standard, explain any deviation:** 0.05

## Define your control and variant
- **Control (A) the current experience, reference your M2 moment of misery and M3 funnel/workflow data:** Standard application entry with past films, new entries and no recommendation option based on the current mood.
- **Variant (B) your single change, copy the relevant screens & functional requirements from your M4 PRD:** Mood chips are visible on the entry screen, selecting a chip filters the rail to that mood
- **Isolation check, what has NOT changed? list everything identical between arms (app version, recommendation engine, notifications, onboarding). If something changed inadvertently, your test is compromised.:** In case chosen to skip no changes to the app and return to the standard screen with past films, new entries and no recommendation option based on the current mood.

## Formalize your hypothesis & shipping criteria
- **Your hypothesis (filled in):** I believe that Mood-Based Entry Point - Pick a mood on login to filter the rail for "The Overwhelmed Browser" A casual-but-invested viewer sitting down for a specific mood (e.g., "quiet Sunday night") rather than a specific title. will result in reducing the friction point of the user choice, allowing to increase 2 metrics: Conversion funnel (30+ sessions) and subscription retention cohort heatmap., as measured by a 5% change in Engagement & Funnel Health (last 90 days) -Homepage Visit → Start Playing within 8 weeks (2 weekly cycles). We will protect User Segment Performance for Power users must not drop throughout the test.
- **Your shipping criteria (filled in):** We will SHIP if Engagement & Funnel Health (last 90 days) -Homepage Visit → Start Playing improves by ≥ 5% at 0.05 and User Segment Performance for Power users must not drop does not reach 0.5 pts. after 8 weeks (2 weekly cycles). We will ITERATE if direction is positive but lift is below MDE. We will KILL if the primary metric shows no improvement or moves negatively. The read date is fixed at the end of 8 weeks (2 weekly cycles), no results reviewed before then.
- **Hardest parameter to define, and did it change your hypothesis? quick debrief:** After pressure test I have adjusted the main metric to reflect properly changes made due to implementation of the feature.
