# Quality Management

Covers "plan and optimize quality of products/deliverables."

## Quality vs. grading

**Quality** is a practice, a mindset, and a process — does the deliverable meet requirements and
fitness for use? **Grading**, by contrast, is just ranking between products/categories of differing
scope or features (a grading distinction isn't a quality problem — a "budget" product can still be
high quality for what it claims to be).

In agile, quality is **customer-centric** (defined through feedback and acceptance criteria); in
predictive/waterfall, it's **process-centric** (defined through planned quality processes and
standards).

## Regulations vs. standards

**Regulations** must be complied with (legally mandatory). **Standards** are guidelines — best
practice, not a requirement, unless a contract or regulation specifically mandates them.

## QA vs. QC vs. audit

- **Quality Assurance:** happens *during* the work, to prevent defects — proactive, process-focused.
- **Quality Control / Review:** happens *after* work is completed, to detect defects via inspection
  and testing — reactive, product-focused. (See the seeded glossary term for this pairing.)
- **Quality audit:** checks how well — and how efficiently — the quality *process itself* is being
  applied (distinct from QC, which checks the deliverable).

To ensure full quality compliance during execution: continually survey the quality of the deliverable,
don't wait for a scheduled checkpoint. For non-compliance found: find the root cause → fix it (may
need a change request) → review/update the process so it doesn't recur. In agile, the retrospective is
where the team digs into the root cause of quality problems and plans fixes together.

## Root cause analysis tools

Fishbone (Ishikawa) diagram, 5 Whys, Why-Why diagrams — all used to trace a defect or non-conformance
back to its actual cause rather than treating the symptom.

## Cost of Quality (see also the seeded COQ glossary term)

- **Cost of conformance:** prevention (training, documentation) + appraisal (testing, inspection) —
  money spent to avoid defects.
- **Cost of non-conformance:** internal failure (rework/scrap, typically via a change request) or
  external failure (liabilities, warranty claims) — money spent because a defect happened.

## Related

- **Kaizen:** continuous improvement, applied to quality processes as much as anything else.
- **Technical debt:** delayed error-correction — the longer it's deferred, the costlier it gets to fix.
- Once the CCB approves a change request, implement it exactly as approved — don't reinterpret or
  "improve on" the approved scope of the change.

## Manage Quality vs. Control Quality (the processes, not just QA vs. QC)

- **Manage Quality:** the broader process of ensuring products, services, and processes meet established
  standards and requirements — this is where the Quality Management Plan gets executed and updated (e.g.
  folding in newly-received building codes/regulations at project start).
- **Control Quality:** measures completeness, compliance, and fitness for use of a product/service
  *prior to final delivery* — inspection and testing live here.
- **Validate Scope** is a distinct, later step from both: it's where the *customer* (not the team) gives
  formal approval that a deliverable meets their requirements. A client simply asking "does it meet
  requirements?" after internal testing is a validate-scope moment, not a signal to reopen quality
  control or dig into the contingency reserve.
- **Inspection vs. audit:** inspections are performed on the *product* (reviewing deliverables, a site
  walkthrough) to check completeness/compliance; audits are performed on the *process* (do project
  activities comply with organizational/project policies and procedures — PMBOK 6th edition, page 294).
  An external quality audit examines process compliance — not budget/schedule status (that's a
  performance review), not defects (that's Control Quality), and not scope-baseline conformance (that's
  Scope Control).
- **When 100% inspection destroys the item being tested** (e.g. a filter that can't be reused once
  tested), order more than needed and run acceptance sampling on the surplus batch, rather than skipping
  inspection or inspecting only after full delivery.

## The seven basic quality tools

Beyond the fishbone/Ishikawa diagram (see Root Cause Analysis Tools above):

- **Checklist:** a list of items/tasks/requirements to verify for consistency and correctness.
- **Check sheet (tally sheet):** records and counts occurrences of specific events or issues.
- **Control chart:** tracks process variation over time to detect potential issues.
- **Histogram:** a vertical bar chart showing how often a variable state occurs (PMBOK 7th edition, page
  189) — e.g. breaking a defect count down by category (bugs, UX, UI, missing features, other). Each bar
  = one category's share.
- **Pareto chart:** a histogram that ranks issues from highest to lowest *frequency*, built on the
  Pareto principle (80/20 rule: 80% of problems come from 20% of causes). Applying it means finding each
  issue's *frequency*, not its impact, urgency, or cause.
- **Run chart:** plots data points chronologically to show trends/patterns over time.
- **Scatter diagram:** shows the relationship/correlation between two variables.
- **Flowchart:** a visual sequence of steps/processes in a system, used to analyze, document, or
  optimize workflows.

## Quality philosophies and techniques

- **Just In Time (JIT):** only acquire/use resources when needed — an *inventory* technique (e.g. don't
  stockpile spare parts; order them as needed) that reduces waste and expiry.
- **Lean management:** the underlying *philosophy* of maximizing customer value while minimizing waste
  (JIT and Kanban are specific techniques/methods that live under this philosophy).
- **Six Sigma:** a data-driven improvement philosophy aimed at reducing the probability of an error or
  defect occurring.
- **Total Quality Management (TQM):** a management philosophy of continuous improvement through
  involving *all* employees in quality goals.
- **Plan-Do-Check-Act (PDCA), Deming Cycle:** an iterative management method for continuous improvement
  of processes or products.
- **Design of Experiments:** controlled tests to understand the relationships between factors affecting
  an outcome.
- **ISO 9000 series:** standards defining an effective Quality Assurance system for manufacturing and
  service industries.

## Cost of Quality, in full

The seeded Cost of Quality (COQ) glossary entry gives the two top-level buckets; here's the four-way
split tested on exam cost-allocation questions:

| Bucket | Type | Examples |
|---|---|---|
| Prevention costs | Cost of Conformance | Training, process documentation |
| Appraisal costs | Cost of Conformance | Testing, inspection, regression analysis, auditing |
| Internal Failure costs | Cost of Non-Conformance | Rework, scrap, refactoring |
| External Failure costs | Cost of Non-Conformance | Liabilities, warranty charges, lost business |

Cost of Conformance = money spent *during* the project to avoid failures. Cost of Non-Conformance =
money spent *during and after* the project *because* failures happened. On an exam question giving a
cost-of-quality breakdown table, match each line item to its bucket by what it actually pays for (e.g.
"Inspection" → Appraisal; "Warranty charges" → External Failure), not by guessing from the total.

## Software-quality vocabulary

- **Bug:** a software flaw/defect causing unexpected behavior — the software-specific synonym for
  Defect.
- **Refactoring:** improving code quality without altering its expected behavior.
- **Regression:** the reappearance of previously-fixed bugs after new changes are made.
- **Unit testing:** testing individual units/components of an application in isolation.
- A found coding-standards violation (a form of technical debt) is neither ignored (that's low
  ownership, not "gold plating") nor fixed unplanned mid-sprint (that compromises the current
  iteration's commitment) — it goes to the **Product Owner as a new product backlog item**, to be
  prioritized like any other work. See
  [../people/agile-roles-and-events.md](../people/agile-roles-and-events.md) for the parallel case of
  handling code clean-up during unused sprint capacity.

## Regulation subtypes

Building on the seeded Regulations vs. Standards glossary entry: regulations split into **de jure**
(formally recognized and established by law/legal authority) and **de facto** (widely accepted,
market/industry-driven, but not officially sanctioned). Receiving updated *de jure* building codes
mid-project is a trigger to update the
Quality Management Plan's standards/specifications — not just the schedule, procurement plan, or
communications plan, since the actual quality bar itself changed.

## Grade vs. quality, revisited

**Grade** (rank/classification, e.g. "economy" vs. "luxury") is a separate axis from **quality**
(conformance to requirements) — see the existing distinction above. A defect is a flaw against
requirements regardless of grade; a low grade is a deliberate scope choice, not a quality failure.
