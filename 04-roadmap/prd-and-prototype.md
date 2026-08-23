# PRD & Prototype Sprint (Module 4)

## Pick & scope with MoSCoW
- **The “Now” feature I’m scoping (name + one-line core description):** Mood-Based Entry Point - Pick a mood on login to filter the rail
- **My finalized Must-Haves (after overriding the AI):** 1) Fixed mood selector (closed set of chips), non-blocking placement — surfaced at login/home but never a full-screen forced gate. A mandatory modal is the single fastest way to violate the Power User guardrail: they already know what they want, and forcing a detour before every session is a direct tax on their 4.8×/week habit.
2) One-tap skip/bypass to standard browse — must be at least as fast as ignoring the feature entirely. This is what protects the guardrail structurally, not just by policy.
3) Rail actually filters on mood selection — the core mechanic; without it there's nothing to measure.
4) Minimum viable editorial mood-tagging — enough curated titles per mood that a selection doesn't dead-end into thin or repetitive results, which would suppress session length rather than grow it.
5) Session-length instrumentation attributed to entry path — every session must be tagged by whether it originated from a mood selection, with duration tracked against the 30-minute threshold. Without this, you cannot report the Primary Metric at all — this isn't a nice-to-have, it's the difference between shipping a feature and shipping an unmeasured guess.
- **What I demoted from Must → Should/Won’t, and why:** Segment tagging on every event (Power / Casual / Wanderer) — not a dashboard, just the underlying data field. You need this in the first sprint because the guardrail requires knowing, from day one, whether Power User behavior moved — waiting until a later sprint to add segment tagging means shipping without the ability to detect a guardrail breach in real time. 

This item have been fully removed simply due to the fact that we are already able to define user type and if the usage of the feature have been initiated or not.

## Generate your Simplified PRD
- **One thing my PRD makes explicit that a vague brief would have missed:** Importance of the feature not covering the initial application features and ability of fast transition to standard search.

## Prompt-to-prototype sprint
- **Where did the prototype reveal a gap in my PRD logic? (what I had to update):** Generally I'm satisfied with the following result as the PRD did solved the main misery point which is allowing to filter available film set using mood based choices with easy access, fast return and cancellations.
- **My shareable prototype URL (Lovable: Share → Share Preview · Bolt: Publish → Web):** https://lovable.dev/preview/l7ZzBqumJYewAz6HfAjjprGroM4ptSkZ
