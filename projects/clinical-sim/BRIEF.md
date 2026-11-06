# ClinicalSim — AI Healthcare Training Platform

## Origin (2026-11-05)
Concept developed in conversation: combine AI patient simulation, EMT scenario coaching, and clinical handoff training into one platform. Inspired by the role/event selection of the BPA practice engine, but designed for healthcare learners. Working name **ClinicalSim**; final branding undecided.

## Vision
Affordable, interactive, profession-specific clinical education using fictional cases, voice/text responses, branching decisions, visual explanations, replay, and targeted feedback. Potential customers: individual learners, EMT/CNA training centers, medical schools and other education programs.

## Initial tracks
- **EMT:** scene and patient assessment, triage, communication, handoff, changing simulated conditions.
- **CNA:** patient communication, routine care, recognizing/reporting changes, safety and positioning.
- **Medical student:** history taking, differential diagnosis, interpretation, management reasoning; anatomy visualizations (e.g., ACL/meniscus) as later educational features.
Each track has different rubric, difficulty and case library but shares a common simulation engine.

## Core experience
1. Choose profession/track, scenario, and difficulty.
2. Read a fictional case with history, symptoms, visuals and available information.
3. Respond by speech, text, or interactive decisions; optionally converse with a virtual patient.
4. See scripted/validated scenario changes and educational visuals.
5. Receive rubric-based feedback, omissions, strengths, decision timeline, and suggested improvements.
6. Replay from a decision point, change an action, compare alternative *simulated* outcomes, and retry.

## Modes
- Guided: hints and checklist, no timer.
- Independent: no hints until after submission.
- Timed: e.g. five minutes to read the case, then a timed response.
- Adaptive: branching cases and reassessment as new findings appear.

## Distinguishing features
- Decision-level error explanations rather than generic grading.
- 'Replay with Correction' showing a decision timeline and educational alternate branches.
- Voice-first interaction, case-based assessment, progress/competency tracking.
- Future video/animated outcomes and 3D anatomy, including orthopedic examples, **not** unreviewed surgical procedural instruction.
- Future instructor dashboard, assignments and cohort analytics.

## Safety and validity
Use synthetic patients only, no identifiable real patient data. Training-only, not real-time medical advice or certification. AI may handle conversation and explanation; validated structured case logic and expert-reviewed rubrics should control scoring and clinical outcomes. Label simulated outcomes as illustrative, not predicted real patient outcomes. Clinical educators must review content before serious deployment. Avoid claiming professional competency based on AI-only grading.

## MVP strategy
Build shared shell for all three tracks but develop **one** high-quality track first; which track is first remains undecided. MVP: role selection, case library, timer, voice/text answers, deterministic branching, feedback, replay, progress. Defer costly generative video and complex 3D until later.

## Constraints
Low startup cost, free/open-source tools where practical, no paid API requirement. Code repository to be created separately by another AI (Grokbot) at owner's direction. This context-hub repo is the shared project specification, not the application code repo.

## Open decisions
First fully developed track; final project name; technology stack; hosting; rubric standards by profession; whether instructor accounts ship in MVP; code repo URL.
