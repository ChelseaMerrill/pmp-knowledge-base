# PMP Knowledge Base

Chelsea's personal study system for the PMP exam (July 2026 exam format). This repo is built to be
used *with* Claude — open it in Claude Code, or point a Claude session at it — not just read on its
own. See [`CLAUDE.md`](./CLAUDE.md) for the full workflow; the short version is below.

## How to use this day to day

**Add something you watched or read.** Drop a new file under `sources/videos/`, `sources/articles/`,
or `sources/guides/` (templates in each folder's README) — paste the transcript, your notes, or a URL.
Then ask Claude: *"process my new sources."*

**Study.** Ask Claude: *"quiz me"* or *"quiz me on risk management"* or *"quiz me on stuff I've been
missing."* Answers can be free text — you don't need to guess at multiple choice.

**Check progress.** Ask Claude: *"give me a weak-areas report."* It reads your quiz history and writes
a dated report to `reports/`, ranking your weakest topics with links back to the notes and sources
behind them.

## Layout

| Path | What lives here |
|---|---|
| `roadmap/` | The 12-week study plan this repo was seeded from, plus a session log |
| `sources/` | Raw inbox — videos, articles, and guides as you ingest them |
| `domains/` | Distilled notes, organized by the three official exam domains |
| `glossary/terms.yaml` | Canonical term list, tagged by domain and originating source |
| `practice/` | Question bank, your attempt history, and a running mistakes list |
| `reports/` | Dated weak-area snapshots |
| `study-guide/guide.md` | Chelsea's own running study guide, added to directly (not source-generated) |

## Exam reference

Built around the PMI Examination Content Outline effective July 2026: **People 33%** / **Process 41%**
/ **Business Environment 26%**, roughly 60% agile/hybrid content. See `roadmap/roadmap.yaml` for the
full week-by-week plan.

---
PMP® and PMBOK® are registered marks of the Project Management Institute, Inc. This repo is an
independent personal study aid and is not affiliated with or endorsed by PMI.
