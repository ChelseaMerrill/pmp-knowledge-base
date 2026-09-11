# Schedule Control and Integrated Change Control

Covers "plan and manage schedule," "develop and manage project scope," and the change-control side of
"develop an integrated project management plan." See the seeded glossary terms for Critical Path
Method, Float/Slack, Crashing, Fast Tracking, Scope Baseline, WBS, and Scope Creep — this note covers
the surrounding mechanics and the process itself.

## Scope: baseline, control, and validation

- The **Scope Management Plan** (part of the Project Management Plan) describes the tools/techniques
  used to manage scope.
- **WBS** is deliverables-oriented — it helps the team visualize and organize the total scope of work.
- **Scope control:** the team verifies deliverables align with requirements.
- **Scope validation:** the *customer* formally approves the deliverables. Control and validation are
  distinct steps — don't conflate the team's internal check with the customer's formal sign-off.
- The PM should never accept a requirement without a defined acceptance criteria — skipping this
  invites conflict with stakeholders later about whether a deliverable actually satisfies the
  requirement.
- Key stakeholders should stay involved through every phase, both to keep them engaged and to secure
  acceptance of deliverables when the time comes.
- The **Scope Statement** (description, deliverables, acceptance criteria, and exclusions — PMBOK 7th
  edition, page 246) is developed from gathered requirements, and precedes the WBS: Requirements →
  Scope Statement → WBS / WBS Dictionary → Execution. See
  [wbs-and-decomposition.md](wbs-and-decomposition.md) for the WBS side of that flow.
- If implemented features later turn out to differ from the scope statement, the document to check is
  the **Requirements Traceability Matrix (RTM)** — it maps requirements to the deliverables that
  satisfy them, documented along with issues and test results (PMBOK 7th edition, page 189).
- A **Work Authorization System** — formal documented procedures for authorizing work — is the fix when
  tasks are being performed out of order/at the wrong time, causing rework and morale problems. It's
  distinct from an org chart, a RACI matrix, or the communications management plan, none of which
  actually govern *when* work is allowed to start.
- The **Assumption Log** records factors treated as true/real/certain without proof (PMBOK 7th edition,
  page 185). When a team's estimate depends on an unverified assumption (e.g. "this will take 2 months
  *if* the third-party system follows the international standard"), document that assumption in the
  log — this is a distinct next step from checking critical-path impact or re-running the estimate.

## Schedule mechanics

- **Lead** and **Lag** are set during the Planning phase (lead = overlap between activities; lag =
  enforced delay between them).
- **Resource leveling:** used for over-allocated resources; it *expands* the schedule to resolve the
  conflict.
- **Resource smoothing:** uses available slack instead of extending the schedule — so it does *not*
  expand the schedule, but only works within existing float.
- The **critical path** is the minimum duration to complete the project; every activity on it has zero
  float, so a slip anywhere on the critical path slips the project finish date.
- **Schedule crashing** (add resources → costs more) and **fast-tracking** (run activities in parallel
  → riskier) are compression techniques used during controlling, and both require a change request.
  When behind schedule, check fast-tracking first, since it doesn't raise cost the way crashing does.

## The Integrated Change Control process

1. A change is raised — a deviation from baselines, a new requirement, or an unmet acceptance
   criterion.
2. The PM creates a change request with an impact assessment/analysis.
3. The PM logs the change into the change log.
4. The PM submits the CR to the **Change Control Board (CCB)**.
5. The CCB reviews and decides: defer, reject, or approve.
6. The PM updates the change log with the decision and informs stakeholders.
7. If approved, the PM updates baselines and implements the change.
8. Monitor the results.

Always evaluate before deciding or acting — include the team, and check with the team/sponsor before
raising a change request in the first place. A **murder board** can also serve as a phase/kill-point
gate deciding whether a project continues past a given stage (see the seeded glossary term).

When a **critical key stakeholder** (e.g. the sponsor) requests a change, treat it with high priority
and issue a change request to the CCB promptly — even a sponsor's request still has to go through the
formal process, rather than being auto-accepted (since they asked) or refused outright (since it's late
notice). If the CCB approves a change but with an implementation method the PM disagrees with, the PM
should implement it as approved — the CCB's decision should be respected and followed through the
integrated change control process, not treated personally. Building a prototype using the PM's
preferred (rejected) method anyway is itself scope creep, since it's work neither requested by the
client nor included in the scope statement.

When multiple CCB members' opinions diverge on a change request, the best path to a decision is
**collaboration/consensus** — open dialogue where differing viewpoints get discussed until the group
commits to a decision (PMBOK 7th edition, page 168) — rather than a vote, or deferring to the most
experienced member or a board director.

## Staffing conflicts in a functional organization

If a PM didn't personally assign their team members (a sign the organization is functional), and team
members are spending less time on the project than their stated availability, threatening the
schedule: the fix is to **negotiate clear, written assignments with reliable scheduling priorities with
the functional managers** — staff assignment is their responsibility, not the sponsor's. Asking the
sponsor for more resources, adjusting the schedule/deadlines, or crashing the project all skip past the
actual root cause (competing priorities set by the functional managers who control the staff).

## Predictive vs. adaptive vs. hybrid, in practice

- **Waterfall (also Traditional, Classical, Predictive, Plan-Based, Linear):** a full plan up front —
  fixed scope, minimal uncertainty; changes are neither easy nor welcome (a thorough, lengthy change
  process); deliverables ship at the end.
- **Agile (also Change-Driven, Iteration-Based, Adaptive):** plan each iteration only; changes are
  very welcome; value is delivered throughout, not just at the end. Agile doesn't route changes
  through a CCB the way predictive does.
- **Hybrid** mixes both — recognizable when a question says so explicitly, or mixes vocabulary from
  both worlds. Always identify which part of the project a scenario is currently in (agile or
  waterfall) and answer from that part's practice, not the other one.
- **Tailoring** happens during planning (and can continue for improvement afterward) — choosing which
  processes/tools suit the project, guided by OPAs/PMO standards.
