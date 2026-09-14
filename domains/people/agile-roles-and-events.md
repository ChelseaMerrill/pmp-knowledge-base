# Agile Roles and Events

Covers the Scrum/agile mechanics that show up across People, Process, and Business Environment
questions — roles, backlogs, ceremonies, and the artifacts each role owns.

## Roles

- **Product Owner (PO):** voice of the customer; prioritizes value; refines and owns the **product
  backlog**; the Single Point of Contact (SPOC) between stakeholders and the development team; owns the
  **product vision** and **product roadmap**. To get value and ROI earliest, the PO's lever is
  prioritizing the backlog — not process improvement or team support (that's the Scrum Master's job).
- **Scrum Master / Team Facilitator:** facilitator, coach, servant leader; removes impediments and
  resolves conflicts. See the glossary's Team Facilitator entry — Scrum Master, project team lead,
  project manager, and team coach are overlapping titles for this same function in agile. As a servant
  leader, when a team member is blocked by something outside their control (e.g. a tool/license
  limitation), the PM/Scrum Master's job is to go resolve it with the relevant stakeholder — not to tell
  the team member to self-solve it or wait for the retrospective.
- **Development Team:** self-organized and cross-functional (diverse skills, no external dependency);
  plans and estimates its own work; owns the **sprint backlog**. Members may be
  **T-shaped** (deep in one area, capable in others, more willing to collaborate) or **I-shaped** (deep
  in one area only); a healthy agile team favors T-shaped members. The team also owns its own
  **sustainable pace** — a pace it can maintain indefinitely.
- **Scrum team** = PO + Scrum Master + Development team together. Scrum rests on 3 **pillars**
  (Transparency, Inspection, Adaptation) and 5 **values** (Commitment, Courage, Focus, Openness,
  Respect).

User stories (US) and acceptance criteria (AC) live in the product backlog (maintained by the PO); the
tasks the team breaks them into live in the sprint backlog (maintained by the team). Both feed the
shared artifacts: increments, the scrum board, and the impediment log. No email between SM/PO/team for
day-to-day coordination — use direct communication instead.

**Scrum of Scrums** coordinates work across multiple teams and Scrum Masters on the same larger
initiative — and is the standard exam answer when one Scrum team has outgrown the ~9-member practical
maximum: split it into two teams and coordinate them with Scrum of Scrums, rather than abandoning Scrum
for a predictive approach. Scrum of Scrums is the lightest-weight member of a broader family of **scaled
agile frameworks** — SAFe (enterprise-level), LeSS (multiple teams, one product), and Disciplined Agile
(lightweight, tailor-your-own-process) are the other commonly-tested ones.

## Work item hierarchy and backlog quality

**Theme → Epic → Feature → User Story**, largest to smallest (see glossary). A **Product Backlog Item
(PBI)** is any single element in the product backlog — feature, story, defect, technical work, etc.

- **Backlog refinement (grooming):** the ongoing process of keeping the backlog accurate, detailed,
  estimated, and prioritized — judged against the **DEEP** criteria (Detailed, Emergent, Estimated,
  Prioritized).
- A well-written user story follows the **3 C's** (Card, Conversation, Confirmation) and should meet
  **INVEST** (Independent, Negotiable, Valuable, Estimable, Small, Testable).
- **Acceptance criteria** are what the PO checks a story against before accepting it at review.
- A **spike** is a special story used purely to research/reduce uncertainty (technical approach,
  requirement, or estimate reliability) — it doesn't itself deliver customer value.
- **Risk-value matrix:** prioritize backlog items by plotting value against risk — highest priority goes
  to high-value/low-risk items, lowest priority to low-value/high-risk items (value is weighted over
  risk-avoidance alone). A **risk-adjusted backlog** folds risk-response work directly into the backlog
  alongside feature work.

## Estimation

- **Story points** are a relative, unitless measure of a story's total effort/complexity — assigned to
  the story **as a whole**, not summed from separate role-based sub-estimates (e.g. "5 points from dev
  + 3 from QA" is the wrong way to build an 8-point estimate; the team estimates the whole story
  together).
- **Relative estimation** (story points, comparing items to each other) is normal agile practice;
  **absolute estimation** assigns a specific time/cost/effort unit to an item without that comparison.
- **Planning poker** (card-based, usually **Fibonacci-sequence** cards: 0, 1, 2, 3, 5, 8, 13, 21…) is the
  standard team estimation technique — the growing gaps reflect growing uncertainty at larger sizes.
- **T-shirt sizing** (XS–XL) is a non-numerical alternative, often used for epics before they're broken
  down small enough for story points.
- **Ideal time/hour/day** = the time a task would take with zero interruptions — distinct from elapsed
  calendar time.

## Definition of Ready vs. Definition of Done

- **DoR (Definition of Ready)** applies at **Planning** — is the story ready to be pulled into the
  sprint? A story that lacks enough detail to execute (e.g. a rewards policy story that doesn't say how
  rewards vary by role) fails DoR and should be pushed back to the backlog, not brought into the sprint.
- **DoD (Definition of Done)** applies at **Review** — does the increment meet the criteria to be
  considered complete? (See the glossary's Definition of Done entry.)
- If the PO **rejects** a demoed feature at review: the right sequence is understand why → update the
  work to address the rejection reasons → move it back to the product backlog for reprioritization.
  Don't delete it (it already has value) and don't auto-carry it into the next sprint backlog (the PO
  still has to reprioritize it against everything else).

## The sprint

- First day: **Planning**. Last day: **Review** (demo) + **Retrospective**. Every day: a 15-minute
  status/impediments meeting (daily standup).
- No urgent/other meetings mid-sprint, and no scope changes mid-sprint — if a change would prevent
  delivering the expected value, the PO cancels the sprint instead of forcing the change in. Short of
  that, the **sprint backlog can still be clarified and re-negotiated** with the PO as the team learns
  more mid-sprint (e.g. unexpected technical complexity) — re-negotiating remaining items keeps the
  sprint goal achievable without a full cancellation.
- Blocking issues surface at the stand-up: find the root cause, then decide the action. The daily
  standup itself is **not** a problem-solving forum — if two members start debating a design/tooling
  decision, time-box it and take it offline with a smaller group right after standup, rather than letting
  it run or opening it to the whole team during the ceremony.
- Stakeholders can attend the Review meeting. The Scrum Master re-energizes the team at the
  Retrospective. When a team member proposes a process tweak (e.g. shortening the sprint length) in
  retro, the Scrum Master's move is to **investigate the cause** behind the suggestion before accepting
  or rejecting it — the real problem might be something else entirely.
- The team aims for **consistent velocity** across sprints. Unfinished work doesn't count toward it,
  and work ends when the budget ends (in a fixed-budget adaptive project).
- **Project vision vs. sprint goal vs. release plan** — a classic exam trap: if a team has fundamentally
  different interpretations of *why* the project exists (not just this sprint or this release), the fix
  is reminding them of the **project/product vision** — the sprint goal only frames the current
  iteration, and the release plan only frames the current release.
- **Adding scope without extending the deadline:** unlike a predictive project, agile doesn't require a
  formal change request to change scope — the PO simply drops or defers lower-priority items to make
  room for newly-prioritized ones. Formal CRs are a predictive-approach reflex that doesn't apply here.
- **When organizational processes (not the team's own agile practices) are what's causing delays and
  rework**, tailor or remove the offending processes directly — don't just add more standup time or wait
  for a root-cause session in retro. Transitioning to agile doesn't mean every inherited process fits;
  customize what doesn't work for the team.
- **Extra capacity finishing a sprint early** should pull the next-highest-priority backlog item, not
  unrequested "nice to have" work (e.g. code clean-up) the customer didn't ask for and doesn't know is
  happening — even well-intentioned unrequested work (paying down technical debt) can cause stakeholder
  dissatisfaction if it displaces backlog items the customer actually prioritized. It isn't scope creep
  (the customer didn't request it), but it does violate their right to prioritize the backlog.

## When a stakeholder disagrees with the PO at Review

If a key stakeholder disapproves of a release the PO just approved at sprint review: the PM's role as
**facilitator** is first to align the PO and the stakeholder on a common decision. If that fails, the
PM supports the **PO's decision** — the PO is accountable for approving deliverables against
acceptance criteria, not the cross-functional team (so don't put it to a team vote) and not the PM's
own judgment call.

## Agile performance measurement

Agile KPIs are **empirical measurements** — decisions based on observation of realistic progress, not
predictions — in contrast to traditional/predictive measurement's focus on outputs and forecasts.

- **Burn-down chart:** tracks remaining sprint work (story points or features); owned by the
  PM/Scrum Master; trending *below* the ideal-burndown line is good, *above* it means the team is
  finishing less than committed. Reading one: total planned minus the last value on the chart = what's
  still unfinished at iteration end.
- **Burn-up chart:** tracks release/project scope completed; owned by the PO; trending *above* plan is
  good.
- If a **release burndown** shows story points *increasing* mid-release with no re-estimation, that
  means work was **added to the product backlog** for that release — not a velocity change either way.
- **Feature chart:** same burndown/burnup mechanic, but counting features instead of story points.
- **Cumulative Flow Diagram (CFD):** a stacked-area chart (Backlog / To Do / In Progress / Done bands
  over time) used to evaluate overall progress and spot flow problems. Read WIP off a widening
  in-progress band; read cycle time and lead time off the horizontal distance a unit of work takes to
  cross the "In Progress→Done" span vs. the full "Backlog→Done" span.
- **Throughput chart:** accepted deliverables over time (e.g. committed vs. completed story points per
  sprint) — shows how consistently the team meets its own commitments.
- **Escaped defects:** defects the team missed that end-users find after release. A rising trend flags a
  testing/quality gap, not just a support-volume issue.
- **Lead time vs. cycle time:** lead time is task-created → task-completed (the full span); cycle time
  is work-started → task-completed (the shorter span inside it).
- **Hawthorne effect exam trap:** measuring only one dimension (e.g. feature-delivery volume) skews team
  behavior toward that dimension at the expense of others (e.g. quality). The fix for "we're shipping
  fast but customers are unhappy with bugs" is adding **customer-satisfaction and quality KPIs** as
  success metrics — not just adding a tech-debt backlog item or discussing feedback at the demo (those
  treat a symptom, not the measurement-driven root cause).

## Frameworks

- **Scrum:** the default framework — incremental delivery via sprints (see Roles/Sprint above).
- **Kanban:** a pull-based, flow-based method (vs. Scrum's timeboxed sprints) that limits
  work-in-progress (WIP) via a Kanban board — the board doubles as an information radiator when posted
  somewhere central and visible. **Scrumban** blends Scrum's structure with Kanban's flow, often used
  when a team is transitioning between the two.
- **Extreme Programming (XP):** speed and simplicity via short cycles and strong technical practices
  (pair programming, TDD).
- **Feature-Driven Development (FDD):** larger-scale projects, short iterations, features as the unit of
  work.
- **Lean:** continuous improvement of existing processes and minimizing waste (see also Value Stream
  Mapping in the glossary).
- **Crystal Family:** a set of approaches that scale in weight/formality with team size and project
  criticality.
- **Blended agile:** a custom hybrid combining elements of two or more of the above — the practical
  reality on many real teams, versus adopting one framework "by the book."
- **Test-Driven Development (TDD) / Behavior-Driven Development (BDD):** technical practices, not
  frameworks in their own right — TDD writes the test before the code; BDD frames behavior in shared,
  readable language so developers, testers, and business stakeholders collaborate on it.

## Iterative vs. incremental vs. full agile

- **Iterative:** goal is to refine the product; scope isn't defined up front; many changes expected;
  relies on experimentation and feedback; delivers at the very end.
- **Incremental:** goal is time-to-market; scope is defined; minimal changes expected; delivers
  completed increments along the way (earlier ROI; can ship after each iteration).
- **Full Agile Approach:** mixes both iterative and incremental.
- **MVP vs. MMP:** MVP (Minimum Viable Product) gets early feedback and minimizes risk; MMP (Minimum
  Marketable Product) speeds up time-to-market.
- **Product vision → product roadmap → release plan** narrow in scope and detail in that order: vision
  is the overall "why," the roadmap sequences milestones across the product's life, and the release plan
  maps the nearer-term delivery detail.

## On "being" vs. "doing" agile

Also called Change-Driven, Iteration-Based, or Adaptive. Three defining characteristics: (1) plan each
iteration only, no advance planning of the whole project, (2) changes are very welcome, (3) value is
delivered throughout the project, not just at the end. *Doing Agile ≠ Being Agile* — following the
ceremonies without the underlying mindset isn't the same as actually being agile.
