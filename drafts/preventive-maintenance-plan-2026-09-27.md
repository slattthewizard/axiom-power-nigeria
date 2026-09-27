---
meta_title: "Preventive Maintenance Plan for Nigerian Industrial Plants"
meta_description: "Build a preventive maintenance plan for a Nigerian industrial plant: asset register, criticality, task lists, spares and a CMMS to track compliance."
primary_keyword: "preventive maintenance plan"
secondary_keywords: "planned maintenance, preventive maintenance schedule, pm programme, condition based maintenance, asset register"
---

# Building a Preventive Maintenance Plan for a Nigerian Industrial Plant

Most plants in Nigeria are not short of maintenance activity. Technicians are busy most weeks, oil gets changed, filters get swapped, and a generator or a pump still fails without warning and takes a shift or a production line down with it. That gap between busy and effective is usually a sign that a preventive maintenance plan exists only as a list of jobs, not as a programme with an asset register, criticality ranking and a way to check whether the work is actually being done.

A preventive maintenance plan is a schedule of tasks, tied to specific assets, performed at fixed intervals or usage triggers, based on what the manufacturer and your own failure history say that asset needs before it fails. Done properly it cuts unplanned trips, extends the life of engines, turbines, pumps and switchgear, and gives a maintenance manager a defensible answer when a director asks why the budget looks the way it does.

This article sets out how to build that plan for a Nigerian industrial site, whether the fleet is a handful of diesel gensets or a mix of turbines, compressors and rotating equipment across a plant.

## Preventive Maintenance vs Reactive and Predictive

Three approaches sit side by side on most sites, and confusing them is the first mistake.

Reactive maintenance means fixing something after it fails. It has a place for low-criticality assets where failure is cheap and safe, but running a plant's critical equipment this way means downtime dictates the maintenance calendar, not the other way round.

Preventive maintenance (PM) means servicing an asset on a fixed schedule, whether time based (every three months) or usage based (every 250 running hours), regardless of its actual condition at that point. It catches wear before failure but can also mean replacing parts that still had useful life left.

Predictive or condition based maintenance uses measured data, vibration, oil analysis, thermography, to decide when an asset actually needs attention rather than working to a fixed calendar. A mature programme layers this on top of PM rather than replacing it. The two approaches, and the techniques behind condition monitoring, are covered in our [companion article on predictive maintenance](/blog/predictive-maintenance/), and most Nigerian plants get the best return by starting with a solid PM base and adding condition monitoring on the handful of assets where a failure is expensive.

None of this needs to reference a specific management standard to work, but if a board wants the programme benchmarked against something recognised, the ISO 55000 family of asset management standards sets out the vocabulary and principles most consultants and auditors work from.

## Start With an Asset Register and a Criticality Ranking

A PM plan without an asset register is really just a set of habits. The register is the foundation: every piece of equipment that gets maintenance attention, listed with its identity (make, model, serial number, location, installed date), its technical data (rated output, duty, key clearances or settings), and a link to its OEM documentation.

Once the register exists, rank each asset by criticality, not by how much attention it currently gets. A practical scoring approach looks at three things:

- Consequence of failure: does it stop production, create a safety or environmental hazard, or just cause inconvenience.
- Likelihood of failure: age, duty cycle, known weak points, history of trips.
- Redundancy: is there a standby unit that covers for it, or does this asset being down mean the whole process stops.

A standby generator with an automatic transfer switch behind it is a different risk than the single steam turbine driving a plant's only compressor train. Criticality decides where the PM budget, the best technicians and the tightest schedule intervals go, and it decides which assets are worth adding condition monitoring to first.

## Build Task Lists From OEM Manuals, Not Generic Checklists

The actual content of a PM task, what to inspect, what to measure, what the acceptable range is, what to replace, should come from the equipment's own operation and maintenance manual, not from a generic template copied across every machine on site. A borrowed checklist for a different alternator or a different compressor frame will miss the specific torque values, clearances and consumable part numbers that manual carries.

Where a manual is missing or the equipment is old enough that documentation has been lost, the OEM's regional office or authorised parts channel is usually the fastest way to recover it. Manufacturer datasheets for equipment of a given class typically show broadly similar service intervals and check points, but the specific machine's own manual always governs over a general rule of thumb.

Each task on the list should state what to do, what tool or instrument it needs, the acceptance criteria (a number or a pass/fail condition, not "check and adjust"), and what to record. A task that just says "check generator" gives a technician nothing to be held to and gives the maintenance manager nothing to audit later.

## Setting Maintenance Frequencies

Frequencies come from three sources: the OEM manual's stated intervals, the manufacturer's severe duty adjustments for heat, dust and continuous running (all common in Nigerian sites), and the plant's own failure history once enough of it has been logged. Where OEM guidance gives a range rather than a fixed figure, Nigerian ambient heat and the harmattan dust season usually justify sitting at the shorter end.

A simplified frequency band, applicable across most rotating and power generation equipment before it is tailored to each specific asset's manual, looks like this:

| Frequency band | Typical scope | Example tasks |
|---|---|---|
| Daily / on shift | Visual and operator-level checks | Fluid levels, leaks, unusual noise or vibration, gauge readings, load |
| Weekly | Light inspection, no shutdown needed | Belt tension, filter indicators, battery condition, control panel alarms log |
| Monthly | Functional tests | Transfer switch test run, load test on standby sets, safety device trip test |
| Quarterly | Minor service | Oil and filter change per OEM schedule, coolant check, connection torque check |
| Annual / major overhaul milestone | Deep inspection, often with a shutdown | Insulation resistance testing, alignment and balancing checks, borescope or internal inspection, calibration of protection relays |

Any task that involves electrical isolation, transfer switch operation, insulation resistance testing on de-energised equipment, or opening a pressurised system must be carried out by qualified personnel working under lockout and tagout with a permit to work in place. This is not optional at any frequency band.

## Spares, Lead Time and the Contract Behind the Plan

A PM schedule that calls for a filter change in week three is only useful if that filter is in the store in week three. Lead time on imported parts, especially for turbine components, alternator parts and some controller boards, can run into weeks, and Nigerian port and customs timelines add to that. Stocking decisions should follow the same criticality ranking used for the asset register: hold the parts that fail predictably and would stop a critical asset if unavailable, and rely on a supplier relationship for the rest.

Where the PM work itself is outsourced, the scope, frequency and reporting obligations should be written into the maintenance contract rather than left as a verbal understanding, and the contract should state what "done" looks like for each visit, not just how often the contractor turns up. Our guide to [what a generator maintenance contract should cover](/blog/generator-maintenance-contract/) goes into the detail of scope, reporting and escalation clauses that make a PM programme enforceable rather than aspirational.

## Running It Through a CMMS

Beyond a handful of machines, a spreadsheet stops being able to track due dates, completed work, parts consumed and technician time reliably. A computerised maintenance management system (CMMS) holds the asset register, generates work orders against the schedule, records what was actually found and done, and produces the compliance data a plant needs.

The features that matter most for a Nigerian industrial site are usually straightforward: offline mobile capture for technicians in areas with poor connectivity, a clear escalation path when a scheduled task is overdue, and reporting that can show compliance percentage by asset and by month without manual collation. A complex system that nobody updates in the field is worse than a disciplined spreadsheet, so match the tool to what the maintenance team will actually use.

## Measuring Compliance and Improving the Plan

The single most useful number in a PM programme is schedule compliance: the percentage of scheduled tasks completed within their due window, by asset and by month. A programme running below roughly 80 to 90 percent compliance is, in practice, not preventing much, because the gaps tend to fall on the assets that are hardest to access, which are often the ones failure would hurt most.

Compliance should be reviewed against actual failure and trip data, not treated as an end in itself. If an asset keeps failing between its scheduled visits, the task list or the interval is wrong for that machine, not the technician doing the work. If a task is completed every time and never finds anything, it may be a candidate for a longer interval or for replacement with a condition based check. The cost of getting this wrong is not abstract: our breakdown of [plant downtime cost per hour](/blog/plant-downtime-cost-per-hour/) sets out how quickly a missed PM task can turn into a production stoppage that dwarfs the maintenance budget that would have prevented it.

A preventive maintenance plan is not a document that gets written once and filed. It is a register, a set of task lists, a schedule and a compliance loop that gets revised as failure data comes in. For plants running a mix of gensets, turbines and rotating equipment, getting the structure right the first time, rather than patching a generic checklist site by site, is what separates a programme that survives staff turnover from one that quietly stops being followed within a year. If you need help building or auditing that structure against your own equipment list, [request a technical proposal](/#contact) and our engineers can scope the assessment through a [power plant audit](/power-plant-audit-nigeria/) against your assets and OEM documentation.

## Frequently Asked Questions

### How is a preventive maintenance plan different from a maintenance schedule?

A schedule is just the calendar of due dates. A plan includes the asset register, the criticality ranking behind it, the task content pulled from OEM manuals, the spares needed to execute it, and the compliance tracking that shows whether it is being followed. The schedule is one output of the plan, not the plan itself.

### How often should preventive maintenance be done on a diesel generator?

It depends on the specific set's OEM manual and its actual running hours, not a fixed calendar figure that applies to every machine. Nigerian heat, dust and continuous duty cycles generally push a site toward the shorter end of the manufacturer's stated interval range rather than the longer end.

### What is a reasonable size to start a PM programme at?

Start with the assets ranked highest on criticality rather than trying to cover the whole site at once. A small number of well maintained, properly documented critical assets delivers more downtime reduction early on than a thin PM effort spread across everything with no depth anywhere.

### Do we need a CMMS, or can we run preventive maintenance on spreadsheets?

A spreadsheet can work for a small fleet with a disciplined team, but it struggles once you need reliable due-date tracking, parts consumption records and compliance reporting across dozens of assets. Most sites outgrow spreadsheets well before they outgrow the rest of the maintenance programme.

### Who should carry out inspections that involve electrical isolation or insulation testing?

Only qualified personnel working under a lockout and tagout procedure with a permit to work in place. This applies regardless of how routine the check feels, and a PM task list should never be written in a way that lets an unqualified person attempt this work unsupervised.
