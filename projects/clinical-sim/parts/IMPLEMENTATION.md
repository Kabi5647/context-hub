# Implementation guidance for next coding AI

## Suggested architecture (proposal, not a decided stack)
Frontend with role selection, case browser, case-reading timer, conversation/action UI, decision timeline, feedback panel, and replay controls. Backend stores synthetic case definitions, case state, decision history, rubric results, and optional user progress. Prefer local/demo mode before authentication. Keep AI dialogue optional and replaceable, with a deterministic non-AI fallback to avoid paid API dependency.

## Example data entities
Track; Case (fictional presentation, findings, assets, learning objectives); Node (state, allowed actions, transitions); Action (student decision, timestamp); RubricCriterion (weight, evidence, feedback); Attempt (history, scoring, mode); Replay (forked attempt). Version case content and scoring rubrics.

## First acceptance criteria
- Three tracks visible, with one complete and two clearly marked as coming soon or sample-only.
- At least one fully playable synthetic case end to end.
- Working five-minute reading phase and separate answer phase; timer settings configurable.
- Text response works without any paid API; voice input progressively enhanced if supported.
- Action timeline and transparent rubric with specific omissions and corrections.
- Replay lets student revise a prior decision and see a predefined alternate scenario branch.
- No actual patient information, no fabricated medical authority, no real-world procedural coaching.
- Mobile-responsive interface, accessible controls, basic automated tests and setup README.

## Future milestones
1. Additional cases and profession-specific rubric libraries.
2. Conversational simulated patients and structured clinical handoff scoring.
3. Educator review workflow and student/instructor dashboards.
4. Expert-reviewed 2D diagrams, then interactive 3D anatomy and carefully reviewed animations.
5. School licensing and usage analytics after validation.

## Developer handoff expectations
Create app code in a **new repository** (not context-hub). Update STATUS and a dated handoff in this hub after development, including code repo URL, architecture, run commands, test results, outstanding risks and exact next steps. Never commit credentials.
