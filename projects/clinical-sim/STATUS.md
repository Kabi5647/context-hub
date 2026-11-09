# ClinicalSim status

Last updated 2026-11-08 (America/Chicago)

Stage: CNA pilot and browser-local guest data controls merged. Foundations, core learner flow, animation, replay, and guest resume are verified. Clinical review and provider-backed accounts are pending.

## Done

- Code lives in the [private ClinicalSim repository](https://github.com/Kabi5647/clinical-sim). [Pilot PR #3](https://github.com/Kabi5647/clinical-sim/pull/3) merged into main at `107fe317670575c62a3681d73609ac9fea2837dd`. It preserves the inherited engine commit from PR #1.
- Retained React, Vite, TypeScript, Zod, Vitest, and oxlint. Added team ownership, roadmap, CI, and case integration contracts.
- Built a responsive landing and training library with EMT, CNA, and Medical Student categories. The introductory fictional CNA pilot supports Guided, Independent, and Timed modes, structured decisions, and confirmed text matches.
- Added deterministic rubric and decision feedback, SVG Stop-on-Error and Consequence playback, and synchronized original/revised comparison. Completed guest results are stored in the current browser with versioned case and rubric IDs.
- [Guest PR #4](https://github.com/Kabi5647/clinical-sim/pull/4) merged into main at `dcc63d27394eec48f082aae447dd831db2404184`. Guests can resume incomplete cases, export structured JSON, and clear local training data after confirmation. Timed deadlines continue while the case is closed.
- Windows build, typecheck, lint, and 31 Vitest tests passed. Edge verified desktop/mobile practice, resume after reload, JSON download, and scoped deletion. [Linux guest PR CI passed](https://github.com/Kabi5647/clinical-sim/actions/runs/42545375420). All 51 tracked files at the PR head matched the locally tested Git blob hashes. The production dependency audit reported zero known vulnerabilities.

## Next

1. Have a qualified clinical educator review CNA content and rubric v1, including the authored branches, and record the decision in the [clinical review record](https://github.com/Kabi5647/clinical-sim/blob/main/docs/clinical-review/cna-communication-v1.md).
2. Define privacy requirements and evaluate provider-backed authentication and authorization. Plan migration tests for new case revisions.
3. Add optional speech and constrained fictional dialogue, then expand CNA, EMT, and Medical Student content.

## Blockers and limitations

- The CNA pilot is Needs Clinical Review. EMT and Medical Student have no playable cases yet.
- Account signup, recovery, and roles await a provider and privacy review for younger learners. Browser-local results can be accessed by users of the same browser profile.
- No public deployment has been approved. Voice and virtual-patient interaction remain future work.
