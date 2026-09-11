# Estimation Techniques

Covers "plan and manage schedule" and "plan and manage finance" — how estimates get built and how
precise they're expected to be at each stage.

## Estimate precision ranges, by project stage

| Estimate type | Also known as | Range | When |
|---|---|---|---|
| Preliminary / Rough Order of Magnitude (ROM) | Rough estimate, Screening estimate, Approximate estimate | −25% / +75% | Beginning of the project, based on historical data from other projects — a high-level estimate, not a precise one. |
| Conceptual / Budgetary | — | −10% / +25% | Narrows down uncertainty by producing a blueprint, prototype, mockup, design, or outline. |
| Definitive | — | −5% / +10% | Determined at the *end* of the planning phase — the most accurate estimate available. |

Precision tightens as the project moves from early feasibility toward baselined planning — a ROM
estimate this early isn't supposed to be accurate to 10%.

A **Basis of Estimates** document describes how an estimate was developed and what information
supported it — regardless of which technique/precision level was used, this is the record of the
reasoning behind the number.

## Estimating methods

- **Analogous Estimating (top-down):** compares to a prior, similar project's total duration/cost —
  fast, less accurate, can be a single point or a range.
- **Parametric Estimating:** multiplies a measurement unit by a rate (e.g. cost per square foot,
  hours per line of code).
- **Bottom-Up Estimating:** estimates individual work-package-level components and rolls them up — the
  most accurate technique, but the most time-consuming.
- **Three-Point Estimating:**
  - *Triangular:* (Pessimistic + Most Likely + Optimistic) / 3
  - *PERT/Beta:* (Pessimistic + 4×Most Likely + Optimistic) / 6 — weights the most-likely value more
    heavily than the simple triangular average. (See the seeded glossary term "Three-Point Estimating
    (PERT)".)
- **Wideband Delphi:** a Delphi variant where the team discusses estimates together after each round
  until they converge (vs. classic Delphi's fully anonymous rounds — see
  [requirements-and-decision-techniques.md](requirements-and-decision-techniques.md)).
- **Agile estimating:** leans on **average velocity** from previous sprints rather than these
  formulas directly, once a team has sprint history to draw on.
- **Expert judgment estimating:** basing estimates on the skill, expertise, or specialized knowledge of
  the project team, independent consultants, or subject-matter agencies — often paired with analogous
  estimating when historical data alone isn't enough.
- **Historical information:** documentation from earlier projects (manuals, requirement specs,
  reports) used as an input to estimating, especially analogous estimating.
- **Single-point vs. Ranged estimating:** single-point produces one value for duration/effort/cost;
  ranged estimating produces a minimum and maximum instead — three-point estimating is a structured way
  to arrive at either.

## Related concepts

- **Alternatives analysis** and **spike** (a timeboxed research investigation) are covered in
  [requirements-and-decision-techniques.md](requirements-and-decision-techniques.md).
- **Sunk cost** — money already spent and unrecoverable — is covered in
  [financial-selection-techniques.md](financial-selection-techniques.md); it should never factor into
  a new estimate or a continue/stop decision.
