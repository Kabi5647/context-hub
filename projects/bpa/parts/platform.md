# Platform

## Source map

- [Private hosted Stride Site](https://stride-bpa-study-kabilen.kabilenmukundhan.chatgpt.site). Owner-only Site audience and application approval were verified; do not infer public access from older handoffs. `?guest=1#practice` remains the memory-only development fixture path and does not bypass hosted access.
- Use the private repository linked in the [project brief](../BRIEF.md#code-repository). Start with its README, `dist/wsap-events.js`, `docs/wsap-research.md`, `dist/presentation-coach.js`, and `worker/auth.mjs`. Use the existing Site configuration when publishing.

## Working constraints

- Keep guest attempts, notes and rehearsals in memory. Account roles currently distinguish student and advisor signup. Advisor signup does not grant access to student records.
- Question practice belongs to objective components. Keep Banking and Finance questions within that event. Use official judging criteria only where verified, and distinguish general self-review from official scoring. Middle Level and state supplements are outside the verified national catalog.
- The rules coach uses deterministic measurements; an optional browser-local model can generate skill quizzes and event-specific critique on compatible desktop hardware. Keep audio temporary, transcription opt-in and local where supported, and content assessment with a human reviewer. Any external AI API needs owner approval, including free APIs.
- Event coverage, year/level filtering and generated content should be labeled according to implementation and evidence. Keep authorized past papers separate from original practice.

## November 14 draft checkpoint

- [PR #1](https://github.com/Kabi5647/BPA/pull/1) contains event plans, 32 original Banking and Finance questions, practice levels, isolated Next/Three introduction and six-character recovery. See the draft's development checkpoint for architecture, tests, asset comparisons and remaining gates.
- Preserve approved accounts, account-scoped progress and server-side Premium gates. A recovery code cannot grant approval or entitlement; only its salted verifier is stored. Codes expire after 30 days, permit five failed guesses and are consumed atomically.
- Real-phone performance and hosted migration remain separate from passing local code tests. No production release of this draft has been made.

## November 15 event-learning checkpoint

- Draft PR #1 head `8a267b5fd2e9c574976acca0d339d4ae28fba714` has 94 event records, 660 official competencies and 46 presentation rubric contexts. Read `docs/curriculum-sources.md`, `docs/practice-content.md`, `docs/learning.md` and `docs/presentation-ai.md` before expanding this implementation.
- Practice packs are generated from readable source and loaded one event at a time. Do not commit the raw PDF, generated full bank, runtime databases or keys. Original questions require independent review. Static lexical candidate alignment leaves 207 explicit skill gaps; never silently fill these with another event or generic questions.
- Completed event history uses immutable account-scoped endpoints and migration 0003. Profile snapshots retain active attempts; do not reintroduce completed-history truncation. Preserve idempotent retry, cursor pagination, identity checks and complete exports.
- The browser reported that its local model cannot run on this hardware. The owner requested preparation of a cloud option only. The documented Cloudflare proposal is synthetic-only initially with $0 additional spend and is not enabled. Verify account/billing/binding support and obtain explicit external-inference approval before any call; student use requires further notices/permissions review.
- Full local build and 78 tests passed, plus legacy regressions; exported source hashes were verified. Current production remains owner-only version 8 without the draft's migrations/features. See the November 15 handoff for remaining release gates.

## November 16 teaching and private-landing checkpoint

- Current draft head `2d4a70fa17a01453a683826d14b238330579badc` provides 274 event lesson placements from 50 teaching modules, each ending with five comprehension items. Read `docs/lessons.md` and `docs/development-2026-11-16.md`; original foundations are shared across related events and do not constitute full instruction for all 660 competencies.
- Practice now has 4,622 event-scoped records, including lesson checks. Static candidate alignment is 480 skills with 180 explicit gaps. Preserve original seed IDs and unreviewed labels. Lesson retakes use stable IDs and immutable archived task identity; avoid changing canonical history serialization without compatibility handling.
- Presentation reports derive evidence-grounded rehearsal plans instead of trusting raw model summaries. Keep human-only review and exact quotations. Saved source-link subsets remain compatible, while unrelated pages and criterion changes reject.
- Explicit `#landing` and View landing page links are authenticated. Retain Sites owner-only sharing plus app approval. Production v8's original source has an authenticated landing fallback, so the permalink can be used after sign-in; the new visible link remains in the draft.
- Full integrated check passed 97 tests and all regressions; all 92 sanitized source hashes were checked. No cloud calls, dependencies, Site deployment, migrations or access expansion occurred.
