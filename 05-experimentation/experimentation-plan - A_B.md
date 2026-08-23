# A/B Experiment Brief, StreamLine (B2C)

## Parameters
| Parameter | Decision |
|---|---|
| Feature under test | Mood-Based Entry Point - Pick a mood on login to filter the rail |
| Persona | "The Overwhelmed Browser" A casual-but-invested viewer sitting down for a specific mood (e.g., "quiet Sunday night") rather than a specific title. |
| Expected outcome | reducing the friction point of the user choice, allowing to increase 2 metrics: Conversion funnel (30+ sessions) and subscription retention cohort heatmap. |
| Primary success metric | Engagement & Funnel Health (last 90 days) -Homepage Visit → Start Playing |
| Baseline rate | 29% |
| Guardrail metric | User Segment Performance for Power users must not drop |
| Guardrail boundary | 0.5 pts. |
| Second guardrail | · |
| Minimum Detectable Effect | 5% |
| Sample size per arm | 1,354 |
| Traffic split | 50/50 |
| Test duration | 8 weeks (2 weekly cycles) |
| Significance threshold | 0.05 |

## Control vs. Variant
- **Control (A):** Standard application entry with past films, new entries and no recommendation option based on the current mood.
- **Variant (B):** Mood chips are visible on the entry screen, selecting a chip filters the rail to that mood
- **Held constant (isolation check):** In case chosen to skip no changes to the app and return to the standard screen with past films, new entries and no recommendation option based on the current mood.

## Hypothesis
> I believe that Mood-Based Entry Point - Pick a mood on login to filter the rail for "The Overwhelmed Browser" A casual-but-invested viewer sitting down for a specific mood (e.g., "quiet Sunday night") rather than a specific title. will result in reducing the friction point of the user choice, allowing to increase 2 metrics: Conversion funnel (30+ sessions) and subscription retention cohort heatmap., as measured by a 5% change in Engagement & Funnel Health (last 90 days) -Homepage Visit → Start Playing within 8 weeks (2 weekly cycles). We will protect User Segment Performance for Power users must not drop throughout the test.

## Shipping criteria
> We will **ship** if Engagement & Funnel Health (last 90 days) -Homepage Visit → Start Playing improves by ≥ 5% at 0.05 and User Segment Performance for Power users must not drop does not reach 0.5 pts. after 8 weeks (2 weekly cycles).
> We will **iterate** if direction is positive but lift is below the MDE.
> We will **kill** if the primary metric shows no improvement or moves negatively.
> The read date is fixed at the end of 8 weeks (2 weekly cycles), no results reviewed before this date.
