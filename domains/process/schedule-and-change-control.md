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
