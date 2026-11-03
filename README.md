# plate

Uday's daily focus system. Plain markdown and CSV, so any model (Claude, ChatGPT, Codex) can read and update it.

## Rules for any model touching this repo
1. Read `CONTEXT.md`, then `PLATE.md`, then the last 3 files in `days/`. Only then plan or answer.
2. Keep to the formats in `days/_TEMPLATE.md` and `weekly/_TEMPLATE.md`. Don't invent new files or folders.
3. Only Uday changes the Active lanes in `PLATE.md`. Models can suggest a change; they don't make it.
4. Every change gets a clear commit message: `day: 2026-11-04 plan`, `day: 2026-11-04 close`, `week: 2026-W45 review`.
5. Never write secrets, employer-confidential details, or health diagnoses into this repo.

## Layout
- `CONTEXT.md` — who Uday is and how to coach him (the "brain file")
- `PLATE.md` — active lanes, background lane, Freezer, Parking Lot
- `days/YYYY-MM-DD.md` — morning plan plus evening close
- `weekly/YYYY-Www.md` — Sunday review
- `metrics/body.csv`, `metrics/content.csv` — numbers for streaks and trends
- `upskill/log.md` — one line per AI-security item studied
- `prompts/` — the morning, evening and weekly prompts (any model can run them)
