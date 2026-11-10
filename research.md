# Research

> EDITING DIRECTIVE: DEVELOPER AND AGENT EDIT THIS FILE COLLABORATIVELY. THE DEVELOPER MUST REVIEW AND APPROVE ITS CONTENT.

Purpose: Keep the evidence, decisions, and current scope that guide the build.

## Working agreement

Developer: Direct the inquiry toward what the next decision needs, judge sources and options, make the consequential decisions, and keep this file current.

Agent: Read the project documents and inspect the project. Help investigate, compare options, and test assumptions quickly. Verify sources directly.

When you begin this step, start a fresh chat so its transcript stays clean. For example:

`Read the project documents and help me research what I need for the next build decision.`

## Inquiry and decisions

Record what informs your build decisions: the questions you investigated, useful sources and what they support, experiments and their results, and the decisions you made with your reasons. Distinguish evidence from assumptions; an Agent's recommendation alone is not evidence.

**Context.** The pitch review raised two points: the game needs a story, and the puzzles may make it too short. I investigated both.

**Reference: Thomas Was Alone** (evidence from [Wikipedia](https://en.wikipedia.org/wiki/Thomas_Was_Alone), [PopMatters](https://popmatters.com/171594-thomas-2495756275.html) and [Engadget](https://www.engadget.com/2013-05-01-thomas-was-alone-review.html)).
- It uses plain geometric shapes. The shapes get personality through color, size and narration. Critics praised the characterization and the introduction of puzzles.
- Some critics found its level design thin compared with its story.
- **Decision:** Use it only as proof that simple shapes can work when the game is fun or the story is understandable. Don't use it as a model for story or puzzles, because its plot and mechanics differ from this game.

**Reference: Sonic 3 & Knuckles and Sonic Mania.**
- **Decision:** Use them as the model for story structure: events in chronological order, zone by zone, with short wordless scenes. This is the Developer's reference. The Agent has not verified how those games tell their stories.

**Story decision.** The scout is looking for lost ghosts, with no deeper meaning. Each area is one event in a sequence, with a short animated moment between areas and a small ending. The tone is cute, with little or no reading.

**Length decision.** The game is short on purpose. The replay reason is seeing the ghosts again, supported by a collection screen where tapping a found ghost replays its animation and sound. Scope comes from depth and polish, not play time.

**Scope options compared.**
- *More ghosts per area* costs new puzzle variations and new ghost animations and sounds. It reuses proven scenery.
- *More areas* costs new scenery, palettes, sound and puzzles. It adds art-style risk, the main risk named in the pitch.
- **Chosen: 3 areas with 4 ghosts each (12 ghosts).** Reasons: lower art risk, a ghost is a small data entry in the data-driven structure, ghosts can be cut individually if time runs short, and it supports the replay reason. This is the Developer's decision. The comparison is the Agent's analysis, not external evidence.

**Puzzle plan (approved by the Developer, draft until tested).** Uses only the three planned types. One type per ghost, with a difficulty twist.

| # | Area | Type | Twist |
|---|---|---|---|
| 1 | 1 | Discover | Obvious glowing object (tutorial) |
| 2 | 1 | Discover | Hidden behind scenery that reacts when tapped |
| 3 | 1 | Order | 3 objects |
| 4 | 1 | Order | 4 objects |
| 5 | 2 | Discover | Hidden, with decoys |
| 6 | 2 | Match | 2 pairs |
| 7 | 2 | Match | 3 pairs |
| 8 | 2 | Order | 4 objects plus a decoy |
| 9 | 3 | Discover | Hidden, with more objects to check |
| 10 | 3 | Match | 3 pairs plus decoys |
| 11 | 3 | Order | 5 objects |
| 12 | 3 | Order + match | Two-step finale using known types |

**Open questions, to settle by playable tests (assumptions, not decided):**
1. How does the player know the order without reading? (Size or brightness, a light or note pattern, or a clue from another object.)
2. How does a match puzzle show a pair? (Shape, color, or sound.)
3. How do hints work? (Glow after idle time, or a button.)

## Scope

### Stretch goals

Unchanged from the pitch, in priority order: 1. fourth area; 2. one or two cause-and-effect puzzles; 3. saving found ghosts between visits; 4. background music; 5. redesigned ghost or more ghost variety.

### Scope changes

- **Added to core:** a chronological story (areas in sequence with short wordless scenes and a small ending); a collection screen where tapping a found ghost replays its animation and sound.
- **Fallback:** build the collection screen with static ghosts first, and add tap-to-replay last in that checkpoint. If Phase 3 is behind schedule, tap-to-replay moves to stretch goals, below saving found ghosts.
- **Changed:** the match puzzle moves from "likely" to core (it appears in 4 of the 12 ghosts). Ghost count rises from 2-3 in the MVP area to 4 per area, 12 in total.
- **Unchanged:** 3 areas, simple geometric art, no cause-and-effect puzzles in core.
- **Why:** the pitch review raised story and length concerns. The change adds depth without adding areas.
- **Follow-up:** update `spec.md` for the story, collection replay, and puzzle behavior.

## Sources and credits

- Thomas Was Alone: referenced for inspiration only; no assets or code used. Sources: [Wikipedia](https://en.wikipedia.org/wiki/Thomas_Was_Alone), [PopMatters](https://popmatters.com/171594-thomas-2495756275.html), [Engadget](https://www.engadget.com/2013-05-01-thomas-was-alone-review.html).
- Sonic 3 & Knuckles and Sonic Mania: referenced for story structure only; no assets or code used.
