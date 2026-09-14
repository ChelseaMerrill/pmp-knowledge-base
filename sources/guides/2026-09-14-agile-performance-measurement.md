---
type: guide
title: "Agile Performance Measurement (Yassine Tounsi, PMP 35 Hours Master Course)"
url: 
date_ingested: 2026-09-14
domain: process
status: processed
---

<!--
Source: a one-page PDF reference sheet ("Agile Performance Measurement") combining short definitions
with example charts (burndown/burnup, cumulative flow diagram, throughput chart, feature chart, escaped
defects, lead time vs. cycle time). This file transcribes the text content; the chart images themselves
are not reproduced, but their shape/axes are described where it matters for understanding the metric.
-->

## Empirical measurements

While traditional project measurements mostly focus on predictions and outputs, Agile measurements focus
on outcomes. Agile KPIs allow data-driven decisions based on a realistic overview of project progress —
known as **empirical measurements** — which supports higher customer satisfaction and optimized
productivity.

## Burn-down chart vs. Burn-up chart

- **Burn-down chart:** demonstrates the remaining work the project team has to complete, illustrated
  with a line that goes downward. Plots story points (or features) remaining, by day, against an ideal
  burndown line.
- **Burn-up chart:** displays the amount of work completed, represented with a line going upward. Plots
  realized work, by day, against an ideal burnup line.

## Feature chart

Displays completed features using a burnup chart, or remaining features using a burndown chart — same
underlying mechanic as a burndown/burnup chart, but tracking features (or story counts) instead of story
points, across sprints, alongside the total number of features in scope.

## Cumulative Flow Diagram (CFD)

Helps evaluate a project's overall progress and identify improvement areas. Plots the number of items
over time as stacked bands per workflow state (e.g. Backlog, To Do, In Progress, Done). The CFD
emphasizes three key metrics, readable directly off the diagram:

- **Backlog:** the top band's growth — how fast new work is being added.
- **WIP (Work In Progress):** the vertical thickness of the "in progress" bands at a given point in
  time — a widening band signals work piling up rather than flowing through.
- **Cycle Time:** the horizontal distance for one unit of work to cross from "In Progress" to "Done."
- **Lead Time:** the horizontal distance for one unit of work to cross the full diagram, from entering
  the Backlog to reaching Done.

## Throughput chart

Shows accepted deliverables over a given period of time, either as a scatter diagram or a bar chart —
e.g. story points **committed** vs. story points of **work completed**, per sprint. Comparing the two
bars per sprint shows how consistently the team delivers against its own commitments.

## Lead time vs. Cycle time

- **Lead time:** the duration of a task from its creation to its completion (the full span: Task
  Created → Work Completed).
- **Cycle time:** how long it takes the team to complete a task once work on it begins (the shorter
  span: Work Started → Work Completed). Cycle time is always a subset of lead time.

## Escaped defects

The number of defects — per unit of time, per sprint, or per release — that the agile team missed or did
not find, which are then detected by end-users after the product release. Tracked over time (e.g.
monthly) as a bar chart of user-reported defect counts; a rising trend signals a quality/testing gap
that predates release, not just a support-volume issue.
