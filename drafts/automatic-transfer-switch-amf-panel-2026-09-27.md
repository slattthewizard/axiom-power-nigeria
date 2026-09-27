---
meta_title: "Automatic Transfer Switch and AMF Panels: How They Work"
meta_description: "How an automatic transfer switch and AMF panel work with your genset controller in Nigeria: transition types, sizing, common faults and testing."
primary_keyword: "automatic transfer switch"
secondary_keywords: "ats panel, amf panel, auto mains failure panel, ats vs changeover"
---

# Automatic Transfer Switch and AMF Panel: How They Work, and Where They Fail

When the grid drops and a factory or hospital loses power without anyone touching a switch, an automatic transfer switch is usually the reason. Paired with an auto mains failure (AMF) panel and the genset controller, it senses the outage, starts the standby set, and moves the load across without a technician standing at the panel. For a plant manager weighing an ATS panel against a manual changeover switch, the decision comes down to how much unattended response the site needs and how the switchgear will be tested once installed.

This article covers how the ATS and AMF panel work together, the three transition types you will be quoted, how to size the switch correctly, the faults that show up most often on Nigerian sites, and a testing routine that keeps the panel trustworthy when it matters.

## What an ATS and an AMF Panel Actually Do

An automatic transfer switch is the piece of switchgear that physically moves the load conductors from one power source to another: normally from the utility (mains) supply to a standby generator, and back again once the mains supply is stable. It is built around two contactors or a single motorised changeover mechanism, interlocked so both sources can never be connected to the load at once.

The AMF panel is the control layer that decides when that movement should happen. It monitors the mains supply for undervoltage, overvoltage, phase loss and frequency drift, and when it detects a genuine failure rather than a brief dip, it sends a start signal to the genset controller. Once the generator has run up and stabilised, the AMF panel commands the transfer switch to close onto the generator side. When mains returns and stays within limits for a set delay, the sequence reverses and the set cools down before shutting off.

On many industrial installations the AMF function sits inside the genset controller itself, from manufacturers such as Deep Sea Electronics or ComAp, rather than in a separate cubicle. Smaller or older sites still use a standalone AMF panel wired between the mains supply, the transfer switch, and a simpler generator controller. Either arrangement does the same job: sense, start, transfer, and transfer back.

## ATS vs Changeover Switch

A manual changeover switch, whether a simple 4-pole rotary switch or a larger air-circuit-breaker interlock, still needs a person to walk to the switch room and operate it once the generator has started. An automatic transfer switch removes that step and adds the sensing and timing logic that decides when a transfer is genuinely warranted, rather than reacting to a momentary sag that would resolve on its own.

The trade-off is complexity and cost of ownership. A manual switch has fewer parts to fail and is easier for site staff to understand at a glance. An ATS panel has sensing relays, timers, and contactors with motor operators or solenoids, all of which need testing on a schedule rather than being checked only when someone happens to operate them. Sites that run unattended overnight, carry life-safety or process loads, or cannot rely on someone reaching the switch room at short notice generally move to an ATS. Sites with a dedicated operator on every shift sometimes stay with a changeover switch and accept the manual step. Our companion piece on the manual option, /blog/changeover-switch-guide/, covers pole configuration, contact ratings and interlocking in more depth.

## Transition Types: Open, Closed and Delayed

The transition type quoted on an ATS panel changes both the price and the electrical design of the switch. There are three in common use.

**Open transition** breaks the connection to the outgoing source before making the connection to the incoming source, so there is a short interruption, typically well under a second once the generator has already stabilised. This is the standard choice for most industrial and commercial standby applications.

**Closed transition** briefly parallels both sources for a fraction of a second during the switch, avoiding any interruption at all. It needs synchronising logic in the controller and a transfer switch rated for the momentary paralleling, so it costs more and demands tighter commissioning. It suits processes that cannot tolerate even a sub-second break, such as continuous production lines with sensitive drives.

**Delayed transition** (sometimes called in-phase transition when timed to the phase angle) adds a deliberate pause of a few seconds between disconnecting from one source and connecting to the other, mainly to let motor loads decelerate before being re-energised. This protects motors and their driven equipment from the inrush and mechanical shock of reconnecting to a live source while a motor is still spinning down, a real risk on sites with several large induction motors on the same bus.

| Transition type | What happens | Typical use |
|---|---|---|
| Open | Brief break between sources | General standby power, most factories |
| Closed | Sources briefly paralleled, no break | Continuous processes, sensitive electronics |
| Delayed / in-phase | Deliberate pause before reconnecting | Buses with large motor loads |

## Sizing an ATS Panel Correctly

An undersized transfer switch is one of the more expensive mistakes on a standby power project, because it usually only shows up as nuisance tripping or contact damage months after commissioning. A few points matter more than the headline current rating:

- **Match the switch rating to the incomer, not just the load.** The ATS should be rated at least equal to the upstream protective device, not simply the calculated running load, so it can carry through-fault current without damage before protection operates.
- **Check the withstand and closing rating (WCR), not only the continuous current rating.** This tells you whether the switch survives a fault current on its terminals for the time upstream protection takes to clear, which matters more on sites fed from a strong grid transformer or a large generator.
- **Confirm neutral switching.** On an earthing arrangement with separate neutral and earth conductors maintained back to source, the ATS normally needs a switched neutral pole (a 4-pole switch) to avoid parallel earth return paths between the mains and generator neutral points.
- **Size for genset step response, not just steady load.** If large motors or transformers start after transfer, the genset and its AVR need to hold voltage and frequency through the step. Our /blog/generator-sizing-guide/ post covers motor starting kVA and step-load allowances.
- **Interlocking.** Mechanical and electrical interlocks that make it physically impossible for both sources to close onto the load at once are not optional extras; they are the safety case for the switch.

## Common ATS and AMF Panel Faults

Most of the calls our engineers get on ATS panels fall into a small number of repeat failure patterns.

| Symptom | Likely cause | What to check |
|---|---|---|
| Generator starts but never transfers | Mains sensing relay stuck reading "healthy," or transfer inhibit input active | Sensing relay output, phase presence on all sensed phases, external inhibit or interlock signals |
| Transfer happens on a brief dip that should not trigger it | Sensing thresholds or time delays set too tight for local grid quality | Undervoltage/overvoltage pickup and delay settings against actual mains behaviour |
| Switch fails to move to either position | Contactor coil open circuit, or motor operator jammed or seized | Coil continuity, control voltage at the coil terminals, mechanical linkage for corrosion or debris |
| Contacts show pitting, burning or a welded contactor | Repeated transfer under load without adequate arc suppression, or a switch undersized for fault duty | Contact surfaces, arc chute condition, correct WCR against actual fault current available |
| Retransfer to mains does not happen after supply is restored | Retransfer time delay not elapsed, or mains sensing not recognising restoration | Timer settings, mains sensing calibration, whether the delay is intentionally long to avoid rapid cycling |
| Nuisance genset starts with no real mains failure | Loose or corroded sensing wiring, or a sensing relay drifted out of calibration | Wiring terminations in the sensing circuit, relay calibration against a known good supply |

A stuck or welded contactor is the fault most likely to strand a site with no power at all, because it can leave the switch neither fully on mains nor fully on generator. It is also the fault most often traced back to a switch undersized for the fault current it actually saw, which is why the withstand rating above is not a paperwork detail.

## Testing and Maintenance

An ATS panel earns trust the same way any protection device does: by being exercised regularly under conditions close to what it will see during a real event, not just inspected visually. A workable routine looks like this.

- **Monthly no-load transfer test.** Simulate a mains failure using the panel's test function, not by pulling a live breaker, and confirm the genset starts, transfers, runs, retransfers and shuts down correctly, timing each stage against the settings on record.
- **Periodic on-load test.** A no-load test proves the logic works; it does not prove the generator can hold voltage and frequency with the actual plant load connected. A load bank test, covered in /blog/generator-load-bank-testing/, confirms the set and the switch perform together under realistic load, not just the small standing load a site carries that day.
- **Contact and contactor inspection.** On a schedule set by the manufacturer's manual and the number of operations recorded, inspect contact surfaces for pitting or discolouration, check torque on power terminations, and confirm the mechanical interlock still moves freely.
- **Sensing calibration check.** Verify undervoltage, overvoltage and phase-loss thresholds against a calibrated test supply where practical, since drifted sensing is a slow failure a simple pass/fail transfer test will not catch.
- **Controller alarm log review.** Most AMF panels and genset controllers log every start attempt, transfer and fault. Reviewing that log periodically, rather than only after an incident, catches intermittent sensing or charging faults early. Our post on /blog/deep-sea-controller-alarms/ explains what common controller alarm codes usually mean and what to record before resetting one.

Any work inside an ATS panel involves live mains and generator terminals in the same cubicle. This is not a task for anyone without electrical isolation training, a permit to work and proper lockout and tagout on both incoming sources before hands go near the terminals. If your maintenance contract does not already specify who is qualified to open this panel, that gap is worth closing before the next test cycle, not after a fault.

For a transfer switch and AMF panel that has never been formally load-bank tested, or one that has started showing any of the fault patterns above, our engineers can carry out a plant assessment covering the switch, the genset controller and the sensing settings together, and size a solution against your actual incomer rating and fault levels. Get in touch to request a technical proposal, or start with our /generator-maintenance-nigeria/ page for what a structured maintenance contract on this equipment typically covers.

## Frequently Asked Questions

### Does every standby generator need an automatic transfer switch?

No. A generator can be connected through a manual changeover switch if a trained operator is available to respond to every outage and the load can tolerate the delay of a manual operation. An ATS becomes worthwhile once a site runs unattended for periods, carries loads that cannot wait for someone to reach the switch room, or needs a documented, repeatable transfer sequence for compliance or process reasons.

### What is the difference between an AMF panel and a genset controller with AMF built in?

Both perform the same sensing, starting and transfer functions. A standalone AMF panel is a separate cubicle wired between the mains supply, the genset and the transfer switch, often used with simpler or older generator controls. A genset controller with AMF built in, common on newer sets, combines engine control, mains sensing and transfer logic in one unit, which reduces wiring but makes that controller a single point that must be sized and configured correctly for the whole sequence.

### How often should an ATS panel be tested?

A monthly no-load test that confirms the full start, transfer, retransfer and shutdown sequence is a reasonable minimum for an industrial site. On-load testing with a load bank, and physical inspection of contacts and terminations, should follow the interval set out in the manufacturer's manual and any maintenance contract in place, since running hours and number of operations affect contact wear more than calendar time alone.

### Can a changeover switch be upgraded to an automatic transfer switch later?

Sometimes, if the existing switch enclosure and conductor sizing have the physical space and rating margin for motorised operators and a control panel, but in many cases it is simpler and more reliable to replace the switch outright with a purpose-built ATS rated for the site's fault levels. A plant assessment that checks the incomer rating, available fault current and cable routing will confirm which route makes sense for a specific switch room.

### Why does our generator start on mains dips that clear themselves in a few seconds?

This is almost always a sensing threshold or time-delay setting that is too tight for the actual quality of the local mains supply, rather than a fault with the switch itself. Reviewing the undervoltage and overvoltage pickup levels and the associated time delays against real recorded mains behaviour, rather than leaving factory default settings in place, usually resolves nuisance starts of this kind.
