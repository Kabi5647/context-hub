# Context Hub

Shared context for every AI model you use. Paste this repo (or `prompt/load-context.md`) into another chat so models start with the same background — no paid APIs.

## Start here (for humans)
1. Open [prompt/load-context.md](./prompt/load-context.md) and paste it into another AI.
2. Name the project (see `projects/_index.md`).
3. That AI must follow [RULES.md](./RULES.md).

## How other AIs must work
Full rules: [RULES.md](./RULES.md)

Short version:
1. Read `CORE.md` → `projects/_index.md` → project `BRIEF.md` + `STATUS.md` → latest `handoffs/`.
2. Do work in the right `parts/` file.
3. Update `STATUS.md` and leave `handoffs/YYYY-MM-DD-<model>.md`.
4. Never invent prior decisions; never use paid APIs; never delete handoff history.

## Layout
```text
CORE.md                 always-on background
RULES.md                hard rules for every AI
prompt/load-context.md  pasteable instruction
projects/
  _index.md
  <slug>/
    BRIEF.md
    STATUS.md
    parts/
    handoffs/
updates/                hub-level changelog
```

## Links
- Repo: https://github.com/Kabi5647/context-hub
- Rules (raw): https://raw.githubusercontent.com/Kabi5647/context-hub/master/RULES.md
- Load prompt (raw): https://raw.githubusercontent.com/Kabi5647/context-hub/master/prompt/load-context.md
- Core (raw): https://raw.githubusercontent.com/Kabi5647/context-hub/master/CORE.md
