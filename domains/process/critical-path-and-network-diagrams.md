# Critical Path and Network Diagrams

Covers "plan and manage schedule" at the mechanical level — how a network diagram gets built and
walked to produce the critical path. See the seeded glossary for Critical Path Method (CPM), Float /
Slack, and Precedence Diagramming Method (PDM); this note covers the surrounding vocabulary and how the
pieces fit together. See [wbs-and-decomposition.md](wbs-and-decomposition.md) for how the activity list
feeding this process gets built, and [schedule-and-change-control.md](schedule-and-change-control.md)
for lead/lag, leveling/smoothing, and compression techniques.

## Network diagram basics

A **network diagram** (built with the **Precedence Diagramming Method**) is a graphical representation
of the project schedule, mapping out all tasks and how they connect. Each **node** represents a
specific activity within the diagram.

## Dependency types (the logical relationship between two activities)

- **Finish-to-Start (FS):** the successor can't start until the predecessor finishes. (Most common.)
- **Finish-to-Finish (FF):** one task can only be completed after the other has been completed.
- **Start-to-Start (SS):** the successor can't start until the predecessor has started.
- **Start-to-Finish (SF):** the predecessor can only finish once the successor has started. (Rare.)

## Dependency categories (why the dependency exists)

- **Mandatory dependency (Hard logic):** non-negotiable — the next task literally cannot start until
  the previous one is done (e.g. you can't paint a wall before it's built).
- **Discretionary dependency (Soft/preferred/preferential logic):** chosen based on the team's
  preference for how work should best flow, not a hard constraint.
- **External dependency:** between a project activity and a non-project activity outside the team's
  control (e.g. a permit from a government agency) — still must be planned around.
- **Internal dependency:** between two project activities that the project team generally has complete
  control over.

## Walking the diagram: forward pass and backward pass

- **Forward Pass:** moves forward through the network diagram to calculate **Early Start (ES)** and
  **Early Finish (EF)** — the earliest each activity can begin and wrap up.
- **Backward Pass:** moves backward through the diagram to calculate **Late Start (LS)** and **Late
  Finish (LF)** — the latest an activity can start/finish without delaying the project's completion
  date.
- **Total Float (Float/Slack):** how much an activity can slip without delaying the project finish —
  calculated as LS − ES, or equivalently LF − EF. Critical path activities have zero float.
- **Free Float:** how much an activity can slip without delaying the **Early Start of its successor**
  specifically (a narrower, more local measure than total float).

## Critical path vs. critical chain

- **Critical Path:** the sequence of activities that determines the project's minimum duration — any
  delay on it directly delays project completion.
- **Critical Chain:** the *longest* chain of activities, but unlike the critical path, it also factors
  in technical dependencies **and resource availability** — so the critical chain can differ from the
  critical path when resource constraints, not just logical dependencies, drive the true bottleneck.

## Schedule documents, by scope

- **Project schedule:** the detailed plan outlining activity durations, milestones, and deliverables
  for a single project.
- **Master schedule:** a broader plan spanning *multiple* projects or operations, rolling up various
  project schedules (including milestone schedules) into one overview.
- **Milestone schedule:** presents milestones with their planned dates only — a high-level view, not
  the full activity-level detail.
- **Project calendar:** identifies the working days and shifts available for scheduled activities
  (distinct from a resource calendar, which tracks a specific resource's availability — see
  [team-resource-management.md](../people/team-resource-management.md)).
- **Schedule forecasts:** predictions of the project's future timeline based on currently available
  information and knowledge.

## Behavioral traps that distort schedule estimates

These describe *why* team members' actual behavior diverges from the schedule as planned — the exam
likes matching the behavior to the name:

| Trap | What happens |
|---|---|
| **Dropped Baton** | An activity isn't ready to start when its predecessor finishes early — the time gained is lost to poor coordination/handoff. |
| **Student Syndrome** | Procrastination eats into the slack built into an activity's duration, since work only really starts near the deadline. |
| **Self-protection** | Workers don't report finishing early, to avoid management raising future productivity expectations. |
| **Parkinson's Law** | Workers use all the time allocated for a task, regardless of how long it actually takes. |
| **Sandbagging** | Workers intentionally underestimate/lower expectations, to later look like they over-delivered. |

All five point toward the same root cause: buffers and estimates get consumed by human behavior, not
just by the work itself — which is part of why schedule and cost reserves exist (see the seeded
Contingency Reserve / Management Reserve glossary term).
