# Competitive Analysis & Journey Map (Module 2)

## Responses
- **Role, who are you solving for? (the specific user segment or profile):** Marcus, the Film Buff:
A 41-year-old cinephile and heavy user who still actively engages with StreamLine but is losing patience with its recommendation logic.
- **Goal, what is this user ultimately trying to achieve?:** He wants to be treated as a person with specific, evolving taste — surfaced with hidden gems — not funneled into an algorithmically inferred genre bucket.
- **Friction, the main barrier (moment of misery) stopping them from succeeding:** The 'Because you watched' row is a joke... I'm not a genre, I'm a person. I miss when a human curator would surface a hidden gem." Marcus hasn't defected yet, which makes him the more urgent persona for the hook's "every month of inaction" framing — he's a still-retained user actively articulating the exact mechanism (BUG-1091's near-duplicate/franchise recommendations) that could turn him into the next Tom.
- **External tools, the outside platforms or tools the user is forced to use:** 1) Friends/Familiy or other bystander support in the recommendation or choice of the film to watch basically a word of mouth
2) Youtube recommendation.
3) We can assume usage of the Google search to find the specific title name based on fuzzy search.
- **The process, the 3 to 5 manual steps the user takes to get the job done:** 1) Ignore the "Because you watched" row entirely. Since it surfaces franchise/genre near-duplicates (BUG-1091), Marcus has learned it isn't worth consulting — he scrolls past it rather than using it as a discovery tool.
2)Seek recommendations outside the platform. Consistent with Sam's stated behavior ("I trust a recommendation from a friend more than the algorithm"), Marcus likely sources his next watch from social circles, critics, or curated lists — channels that exist outside StreamLine's product surface entirely.
3) Re-enter StreamLine only once he already knows the exact title. This is corroborated directly by the search data (UXR-07, BUG-1080): natural-language/descriptive search fails, and only exact-title matching works. So the workaround isn't "search StreamLine to discover" — it's "decide externally, then use StreamLine's search bar as a lookup tool."
4) Watch, then return to step 1. Because the row never improves on the next visit (it's structurally tied to recent-watch genre, not taste), the cycle resets every session rather than getting smarter over time.
- **Core frustration, the exact moment the process feels most “broken”:** It converts StreamLine from a discovery product into a hosting product — Marcus does the taste-matching work himself, elsewhere, and only routes the final "play" action through the platform. That's the opposite of the value a recommendation engine is supposed to add.
- **The evidence, a specific quote or behavior from the research that proves this:** "I trust a recommendation from a friend more than the algorithm." - UXR - 10
"I trust a recommendation from a friend more than the algorithm." - UXR - 04
"The 'Because you watched' row is a joke, it recommended three more action sequels because I watched one. I'm not a genre, I'm a person. I miss when a human curator would surface a hidden gem." - UXR - 02
- **📎 Your journey map, a shareable link, or the map file you committed (e.g. journey-map.html):** _(not filled in)_
