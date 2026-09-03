# Videos

One file per video you watch. Since Claude can't watch a video directly, paste the transcript (most
platforms — including YouTube — let you copy one) or your own notes taken while watching. A link
alone isn't enough to process.

Name files `YYYY-MM-DD-short-title.md`. Template:

```markdown
---
type: video
title: 
url: 
date_ingested: YYYY-MM-DD
domain: people | process | business-environment | mixed
status: raw
---

<!-- paste transcript or your notes below -->
```

Once you've added a file, ask Claude to "process my new sources" (or name the file) — it'll fold the
content into `domains/`, add new terms to `glossary/terms.yaml`, generate quiz questions into
`practice/questions.yaml`, and flip this file's status to `processed`.
