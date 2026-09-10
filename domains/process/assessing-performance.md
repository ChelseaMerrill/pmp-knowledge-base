# Assessing Project Performance

Covers "evaluate project status." Extends the seeded EVM formula set (PV, EV, AC, CV, SV, CPI, SPI,
EAC, ETC, TCPI) — see glossary for those — with the two terms it's missing and how to read the
combined signal.

## The full EVM term set

Add to the seeded list: **BAC** (Budget at Completion — the total planned budget) and **VAC**
(Variance at Completion = BAC − EAC, telling you the expected over/under at project end).

## Reading CV and SV together

- **CV > 0 and SV > 0** (equivalently CPI > 1 and SPI > 1): ahead of schedule *and* under budget.
  Resource leveling or even crashing can be considered here if there's a reason to use the slack
  productively — the project has room.
- **CV < 0 and SV < 0** (CPI < 1 and SPI < 1): behind schedule *and* over budget. Crashing and
  schedule extension aren't good options here — they add cost you don't have room for. Consider
  fast-tracking instead, and address the root cause of the variance.

## On a performance variance generally

Find the root cause first, then take corrective or preventive action — don't jump straight to a
schedule-compression technique without understanding why the variance happened.

## Related financial metrics

Cost-Benefit analysis, IRR, NPV, and Payback Period are covered in
[financial-selection-techniques.md](financial-selection-techniques.md) — used to make the case for a
solution to stakeholders, or to compare/select between projects, rather than to track an in-flight
project's performance (that's what EVM is for).
