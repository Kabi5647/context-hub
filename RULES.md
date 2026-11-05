# Rules for every AI using this hub

These are hard requirements. If you cannot follow them, say so before doing project work.

## 1. Load before you invent
1. Read `CORE.md`.
2. Read `projects/_index.md`.
3. Open only the project the owner named (or the one clearly in scope).
4. Read that project's `BRIEF.md` and `STATUS.md` fully.
5. Read the newest 1–3 files in `handoffs/` (by date in the filename).
6. Open only the `parts/` files you will actually edit.

Do not invent prior decisions that are not in those files. If something is missing, ask or mark it as unknown in your handoff.

## 2. Stay in your lane
- Work on one project per turn unless the owner says otherwise.
- Prefer editing existing `parts/` files over creating random new docs.
- Do not delete handoffs or rewrite history. Append / update instead.
- Do not spend money, call paid APIs, or require paid tools.
- Do not treat chat memory as source of truth — this repo is.

## 3. Update the shared state every time you finish
Before you end:
1. Update `projects/<slug>/STATUS.md` (Done / Next / Blockers / date).
2. Add a new handoff: `projects/<slug>/handoffs/YYYY-MM-DD-<model>.md`
3. If you created a new project, add a row to `projects/_index.md` and a line in `updates/YYYY-MM-DD.md`.

## 4. Handoff format (required)
Use this shape:

```md
# Handoff — <Model> — YYYY-MM-DD

## Context loaded
- BRIEF / STATUS / which parts / which prior handoffs

## Did
- Concrete changes (files touched)

## Decisions
- What you chose and why (short)

## Next for whoever follows
1. First concrete step
2. Second step
3. Optional third step

## Blockers / questions
- None, or list them
```

## 5. How to talk in this hub
- Be clear and practical; leave steps another model can execute without you.
- Prefer small shippable progress over big rewrites.
- If the owner’s request conflicts with `BRIEF.md`, flag the conflict in STATUS and the handoff — do not silently override the brief.
