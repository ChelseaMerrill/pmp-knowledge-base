# WBS and Decomposition

Covers "develop and manage project scope" — how the WBS gets built, what makes one well-formed, and
the components underneath a work package. See the seeded glossary for Work Breakdown Structure (WBS),
WBS Dictionary, and Scope Baseline; this note covers the surrounding structure and vocabulary.

## What a WBS is

A hierarchical decomposition of the total project scope into smaller, manageable components — work
packages that define deliverables, tasks, and responsibilities. It's **deliverables-oriented**, not
activity-oriented: WBS components describe *what* gets produced, not the steps to produce it.

**Decomposition** is the act of breaking deliverables down into smaller, more detailed, manageable work
packages to build the WBS.

## WBS characteristics

A well-formed WBS is:

- **Definable:** clear description of the work and deliverables.
- **Manageable:** small enough to be effectively controlled.
- **Estimable:** allows accurate time, cost, and resource estimation.
- **Measurable:** clear criteria to track and verify completion.
- **Independent:** minimal overlap or dependencies with other components.

## The MECE principle

**Mutually Exclusive, Collectively Exhaustive** — two properties a good WBS must have:

- **Mutually Exclusive (independent):** no work package overlaps with another.
- **Collectively Exhaustive (the 100% rule):** the WBS captures 100% of the project's required work,
  with no gaps or missing components.

A WBS that violates Mutually Exclusive has duplicated/overlapping work packages; one that violates the
100% rule is missing scope entirely — both are structural defects the exam likes to test by showing a
malformed WBS diagram.

## The components, top to bottom

- **Control account:** a management control point where scope, schedule, and budget are integrated and
  compared to earned value for performance measurement — sits above the work package level, grouping
  related work packages.
- **Planning package:** a WBS component *under* a control account, used to plan and track activities
  that aren't yet fully defined (i.e. scope is known at a high level but not yet decomposed into work
  packages).
- **Work package:** the lowest level of a WBS branch — specific tasks and deliverables within a defined
  scope, budget, and timeline. This is the level estimating and assigning responsibility actually
  happens at.
- **Code of accounts:** the lettering/numbering system that gives each WBS component a unique
  identifier (e.g. 1.1, 1.2, 2.1 in a Tiny House WBS's Planning/Design/Construction/Closeout phases).

## Related scope documents

- **Scope Statement:** the description of the project scope, major deliverables, and exclusions —
  includes the scope description, deliverables, acceptance criteria, and exclusions (PMBOK 7th
  edition, page 246). Built from gathered requirements, and precedes the WBS in the planning sequence:
  Requirements → Scope Statement → WBS / WBS Dictionary → Execution.
- **Activity list:** a detailed list of all planned project activities, built from the WBS's work
  packages.
- **Activity attributes:** the elements tied to each scheduled activity — activity codes, predecessor/
  successor activities, logical relationships, leads and lags, resource requirements, imposed dates,
  constraints, and assumptions.

See [critical-path-and-network-diagrams.md](critical-path-and-network-diagrams.md) for how activities
get sequenced and scheduled once the WBS/activity list exists, and
[schedule-and-change-control.md](schedule-and-change-control.md) for scope control/validation and the
change control process.
