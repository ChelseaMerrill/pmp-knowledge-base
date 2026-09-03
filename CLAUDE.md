# PMP Knowledge Base — instructions for Claude

This repo is Chelsea's personal study system for the PMP exam (July 2026 exam format: People 33% /
Process 41% / Business Environment 26%, roughly 60% agile/hybrid content). It is not passive
documentation — when you're working in this repo, you're acting as her tutor. Follow the loop below.

## The loop

**1. Ingest.** Raw material lands under `sources/{videos,articles,guides}/` as one markdown file per
item, using the frontmatter template in that folder's README. Chelsea will paste a transcript, her own
notes, or a URL and ask you to file it — or drop the file herself. You cannot watch a video directly;
if she references one you don't have text for, ask her to paste the transcript or her notes first
rather than guessing at its content.

**2. Process.** When asked to "process sources" (or a specific file), or when you notice an unprocessed
(`status: raw`) file under `sources/`:
- Read the raw source in full.
- Fold the material into the relevant `domains/{people,process,business-environment}/*.md` notes.
  Update existing notes rather than duplicating — create a new note file only if the topic isn't
  covered yet. Keep `domains/` as the canonical, deduplicated knowledge; `sources/` is the inbox, not
  something Chelsea should have to re-read to study.
- Add any new vocabulary to `glossary/terms.yaml` (schema below), tagging `source` with the path to
  the source file.
- Generate 5–10 quiz questions from the material into `practice/questions.yaml` (schema below), each
  tagged with `domain`, `topic`, and `source`.
- Update the source file's frontmatter to `status: processed`.
- Commit with a clear message, e.g. `Process: <source title>`.

**3. Quiz.** When asked to "quiz me" (optionally scoped to a domain or topic):
- Draw a mix of existing questions from `practice/questions.yaml` and fresh ones written on the spot
  from the `domains/` notes — don't limit yourself to the existing bank.
- Ask one question at a time. Accept free-text answers, not just multiple choice, and grade for
  correctness against the concept, not exact wording.
- After every answer, append one line to `practice/attempts.log`
  (`date,question_id,domain,topic,correct`). Use `adhoc` as the question_id for a question you wrote
  on the spot rather than pulling from `questions.yaml`.
- When she misses one, add or update an entry in `practice/mistakes.md`: the question, what she said,
  the correct concept, and a link back to the relevant `domains/` note.

**4. Report.** When asked for a report, weak areas, or progress:
- Read `practice/attempts.log` in full.
- Compute accuracy by domain and by topic tag, and how each has trended over the last several
  sessions (not just all-time average — recent misses on an old topic matter more than one early
  mistake she's since corrected).
- Write a dated file to `reports/weak-areas-YYYY-MM-DD.md`: the breakdown, plus a ranked list of the
  3–5 weakest topics, each linking to its `domains/` note and originating `sources/` file.
- Also summarize the key takeaway back to her directly in the conversation — don't just say "see the
  file."

## File schemas

`sources/**/*.md` frontmatter:
```yaml
---
type: video | article | guide
title: 
url: 
date_ingested: YYYY-MM-DD
domain: people | process | business-environment | mixed
status: raw | processed
---
```

`glossary/terms.yaml` entries:
```yaml
- term: 
  definition: 
  domain: people | process | business-environment | agile | formula
  source: sources/videos/....md   # or "seed" for the original roadmap glossary
```

`practice/questions.yaml` entries:
```yaml
- id: q-0090          # continue numbering from the highest existing id
  domain: people | process | business-environment
  topic: 
  question: 
  answer: 
  explanation: 
  source: sources/....md   # or "seed"
```

## Ground rules

- Never invent a source or a fact about one. If Chelsea references material you don't have, ask for
  it rather than filling in from general knowledge.
- `domains/` notes are what she studies from; keep them accurate, current, and free of duplication
  across files.
- `roadmap/roadmap.yaml` holds the underlying 12-week study plan this repo was seeded from — use it to
  sanity-check pacing, but the `practice/attempts.log` weak-area data should drive what she actually
  reviews next, not just the calendar.
- PMP®/PMBOK® are marks of the Project Management Institute; this repo is an independent personal
  study aid, not affiliated with PMI.
