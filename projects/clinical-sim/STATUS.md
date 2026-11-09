# ClinicalSim status

Last updated 2026-11-09 (America/Chicago)

Stage: Phase 4 educator demo merged into private main. Five fictional cases remain playable across CNA, EMT, and Medical Student. All five cases and dialogue revisions remain Needs Clinical Review.

## Done

- [Phase 4 PR #7](https://github.com/Kabi5647/clinical-sim/pull/7) merged at `d92d2a8809ce182652cce13338a600b0a431ad75`. Integration head `227e7c7ff044890675fe58087397bdde3c718972`. The 116-file source tree matches the verified local integration.
- Added an Educator Demo with a synthetic roster, groups, classroom management, version-pinned assignments, deterministic completions, progress analytics, feedback, follow-up drafts, and scoped export, clear, and reset.
- Added exact-revision clinical review inspection and local demo comments and corrections. The existing review registry and its approval gate remain authoritative.
- Preserved all five case files, engine, dialogue and guest storage. Original attempts determine completion. Corrections and educator comments remain separate from original scoring.
- Documented future server identity, tenant authorization, privacy and consent decisions, migration, retention, deployment prerequisites, and a threat model in `docs/EDUCATOR-ARCHITECTURE.md`.
- Verified typecheck, lint, production build, 114 Vitest checks, and 12 Chromium journeys. Both npm audits reported zero known vulnerabilities. [Linux PR CI](https://github.com/Kabi5647/clinical-sim/actions/runs/42622045067) · [Linux main CI](https://github.com/Kabi5647/clinical-sim/actions/runs/42622307446).

## Next

1. Assign qualified educators to review every exact case, rubric, and dialogue revision.
2. Validate educator and learner workflows with synthetic records, physical devices, and assistive technology.
3. Resolve age eligibility, consent, sharing, retention, deletion, and institutional access with the owner before configuring production identity.
4. Keep voice device verification and live AI approval separate from the classroom pilot.

## Blockers and limitations

- Clinical sign-off is pending for all five case and dialogue revisions.
- The Educator Demo uses a shared browser profile and synthetic records. Real classroom authorization, production accounts, live AI activation, and public deployment remain gated.
