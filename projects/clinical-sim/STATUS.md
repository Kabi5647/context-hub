# ClinicalSim status

Last updated 2026-11-09 (America/Chicago)

Stage: Phase 3 virtual-patient encounters merged into private main. Five fictional cases are playable across CNA, EMT, and Medical Student. All five cases and dialogue revisions need qualified clinical review.

## Done

- [Phase 3 PR #6](https://github.com/Kabi5647/clinical-sim/pull/6) merged into main at `5ec16063249d1da92c26b833910c51722b269af6`. Integration head `06b9930da87bdd47f2a8ddd71159903b08c642c2`. The five Phase 2 scenario files and the deterministic engine remained byte-identical.
- Added authored virtual-patient dialogue to all five cases, with 17 intents, 34 wording options, controlled ambiguity and unsupported fallbacks, and confirmed-action disclosure gates.
- Added a patient conversation panel with Guided starters, keyboard and mobile support, explicit action confirmation, and a deadline policy that discards late replies.
- Default dialogue uses authored responses. The local mock and optional disabled server adapter select authored response IDs, with validation and bounded failure handling. No live provider was activated.
- Versioned guest transcripts store recognized fictional questions and exact replies. Replay uses the recorded wording and marks responses superseded if a correction removes their disclosure basis. Export and deletion remain local and usable.
- Added an optional on-device voice prototype with an explicit capability check, start and stop controls, editable preview and text fallback. Voice behavior was tested using API doubles and unsupported-browser fallback.
- Verified 98 Vitest tests, nine Chromium journeys, typecheck, lint, and production build. All 29 curated prompts matched their expected facts and authored replies or fallbacks. Both npm audits reported zero known vulnerabilities. [Linux PR CI](https://github.com/Kabi5647/clinical-sim/actions/runs/42570997212)

## Next

1. Have qualified educators review every case and dialogue revision, including permitted variants, disclosure, uncertainty, and fallback wording.
2. Verify physical microphone use and assistive technology on supported devices. Retain the text-first guest path.
3. If the owner approves live AI, validate the server bridge, retention, credential handling, and deployment-wide usage and spending limits before activation.
4. Define eligibility, consent, authorization, retention and deletion requirements before production account work.

## Blockers and limitations

- Human clinical approval is pending for all five case and dialogue revisions.
- Production accounts, live-provider activation, and public deployment require explicit owner approval. Browser-local guest records and bundled case material are inspectable by people with access to the browser profile.
