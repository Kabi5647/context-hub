# Platform

## Source map

- [Private hosted Stride Site](https://stride-bpa-study-kabilen.kabilenmukundhan.chatgpt.site). Owner-only Site audience and application approval were verified; do not infer public access from older handoffs. `?guest=1#practice` remains the memory-only development fixture path and does not bypass hosted access.
- Use the private repository linked in the [project brief](../BRIEF.md#code-repository). Start with its README, `dist/wsap-events.js`, `docs/wsap-research.md`, `dist/presentation-coach.js`, and `worker/auth.mjs`. Use the existing Site configuration when publishing.

## Working constraints

- Keep guest attempts, notes and rehearsals in memory. Account roles currently distinguish student and advisor signup. Advisor signup does not grant access to student records.
- Question practice belongs to objective components. Keep Banking and Finance questions within that event. Use official judging criteria only where verified, and distinguish general self-review from official scoring. Middle Level and state supplements are outside the verified national catalog.
- The coach uses deterministic counts, approximate pace, chosen time limits and fixed prompts. Keep audio temporary, transcription opt-in and local where supported, and content assessment with a human reviewer. Any external AI API needs owner approval, including free APIs.
- Event coverage, year/level filtering and generated content should be labeled according to implementation and evidence. Keep authorized past papers separate from original practice.

## November 14 draft checkpoint

- [PR #1](https://github.com/Kabi5647/BPA/pull/1) contains event plans, 32 original Banking and Finance questions, practice levels, isolated Next/Three introduction and six-character recovery. See the draft's development checkpoint for architecture, tests, asset comparisons and remaining gates.
- Preserve approved accounts, account-scoped progress and server-side Premium gates. A recovery code cannot grant approval or entitlement; only its salted verifier is stored. Codes expire after 30 days, permit five failed guesses and are consumed atomically.
- Real-phone performance and hosted migration remain separate from passing local code tests. No production release of this draft has been made.
