# ClinicalSim status

Last updated 2026-11-08 (America/Chicago)

Stage: Phase 2 merged into the private application repository. Five fictional exercises are playable across CNA, EMT, and Medical Student. All five are Needs Clinical Review.

## Done

- [Phase 2 PR #5](https://github.com/Kabi5647/clinical-sim/pull/5) merged into main at `d7b9e5add5b5f32ba4f60867cb63ed5213af52bc`. Integrated head `b5e67654dbf78fcd4934d0d1b97b034f6f88b88d`. Preserved the original CNA case, rubric, deterministic grading and browser-local data contract.
- Added the EMT recreation-center handoff, medical-student knee history and differential exercise, CNA near-slip reporting, and CNA privacy and hand hygiene. Each has versioned objectives, actions, rubric, authored branches, and a revision-matched review record.
- The catalog validates every authored case and requires a credentialed, dated review event with resolved corrections for an Approved status. All five cases are pending qualified human review.
- Added track-specific SVG environments, observation and timing panels, phase cues, case search, and keyboard-stable landing preview. Replay aligns actions around the correction and compares rubric changes and objectives.
- Guest learning summaries include case and track results, repeated feedback, and trends after three comparable original runs. Revisions remain separate from original-run summaries. Added the [account architecture proposal](https://github.com/Kabi5647/clinical-sim/blob/main/docs/ACCOUNT-ARCHITECTURE.md) covering local storage, roles, sessions, synchronization, privacy, and migration.
- Verified Windows typecheck, lint, production build, 44 Vitest tests and seven Edge Playwright journeys. [Linux Chromium PR CI passed](https://github.com/Kabi5647/clinical-sim/actions/runs/42556614900). Both npm audits returned zero known vulnerabilities at the checkpoint. All 70 tracked files matched the tested local source.

## Next

1. Assign qualified clinical educators to the five exact case and rubric revisions and record their corrections and decisions.
2. Define age eligibility, consent, educator access, retention, and deletion before selecting or implementing production identity.
3. Add case content and assistive technology coverage after review. Keep earlier revisions for saved results and add migration tests when changing a rubric.

## Blockers and limitations

- Qualified clinical educator approval is pending for every exercise. Provider-backed accounts, voice and authored dialogue, and production deployment are future work.
- Guest analytics are browser-local practice data. Keyboard, semantic controls, and reduced motion were checked in the browser suite. Real-device assistive technology validation remains open.
- Production authentication and public deployment require explicit owner approval.
