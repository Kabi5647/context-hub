# Platform

## Source map

- [Public Stride Site](https://stride-bpa-study-kabilen.kabilenmukundhan.chatgpt.site). The guest entry uses `?guest=1#practice`.
- Request access to the current Stride source through the owner. Start with its README, `dist/wsap-events.js`, `docs/wsap-research.md`, `dist/presentation-coach.js`, and `worker/auth.mjs`. Use the existing Site configuration when publishing.

## Working constraints

- Keep guest attempts, notes and rehearsals in memory. Account roles currently distinguish student and advisor signup. Advisor signup does not grant access to student records.
- Question practice belongs to objective components. Keep Banking and Finance questions within that event. Use official judging criteria only where verified, and distinguish general self-review from official scoring. Middle Level and state supplements are outside the verified national catalog.
- The coach uses deterministic counts, approximate pace, chosen time limits and fixed prompts. Keep audio temporary, transcription opt-in and local where supported, and content assessment with a human reviewer. Any external AI API needs owner approval, including free APIs.
- Event coverage, year/level filtering and generated content should be labeled according to implementation and evidence. Keep authorized past papers separate from original practice.
