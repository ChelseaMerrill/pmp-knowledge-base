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
| `notes/notes.md` | One running notes page — Claude appends to it on request as Chelsea learns things |

## Exam reference

Built around the PMI Examination Content Outline effective July 2026: **People 33%** / **Process 41%**
/ **Business Environment 26%**, roughly 60% agile/hybrid content. Predictive/adaptive/hybrid approaches
are woven through all three domains, not isolated to one. See `roadmap/roadmap.yaml` for the full
week-by-week plan, and each `domains/*/README.md` for the full task/enabler breakdown per domain.

**Format:** 180 questions (170 scored + 10 unscored pretest), 240 minutes, two 10-minute breaks. Mixes
multiple-choice (single and multi-response), case/scenario sets, graphic-based, drag-and-drop/enhanced
matching, point-and-click, and pull-down questions. In-person (Pearson VUE) or online proctored
(OnVue).

**Eligibility:** one of four education+experience combinations (all experience within the last 10
years) — e.g. a bachelor's degree + 36 months/3 years leading projects, or a GAC-accredited degree +
24 months/2 years. Also requires 35 hours of PM-relevant commercial training (an active CAPM waives
the documentation for this). See the full table in
`sources/guides/2026-09-08-pmp-exam-content-outline.md`.

**Retakes & renewal:** up to 3 attempts within your 1-year eligibility window; 3 failures means a
1-year wait before reapplying (no wait if the window just expires). Once certified, maintain the PMP
with 60 PDUs every 3 years (CCR).

---
PMP® and PMBOK® are registered marks of the Project Management Institute, Inc. This repo is an
independent personal study aid and is not affiliated with or endorsed by PMI.
