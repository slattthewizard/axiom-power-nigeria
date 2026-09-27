---
meta_title: "Generator Synchronization: How Genset Paralleling Works"
meta_description: "Generator synchronization explained: sync conditions, synchronizing panels, load sharing and common faults on paralleled gensets in Nigeria."
primary_keyword: "generator synchronization"
secondary_keywords: "generator synchronizing panel, generator paralleling, load sharing, synchronising generators"
---

# Generator Synchronization: How Genset Paralleling and Load Sharing Work

A single generator carrying a whole plant load has one obvious weakness. The day it needs a filter change, an injector swap or an unplanned repair, the site either has no backup or goes dark while the work is done. Generator synchronization is how a plant avoids that choice. Two or more sets are brought to matching voltage, frequency and phase, closed onto a common bus, and then made to share the load, so that any single machine can be pulled off for service without interrupting supply.

For a maintenance manager, synchronization is not a control-room curiosity. Get the sync conditions wrong, or leave the load sharing settings poorly tuned, and the result is a nuisance trip at best and a damaged alternator at worst. This article sets out what synchronizing generators actually checks before a breaker closes, how manual and automatic synchronizing panels differ, how load is divided once sets are paralleled, and the faults that turn up most often on sites running long hours on variable load.

## Why Sites Parallel Generators at All

A plant running two 500 kVA sets in parallel gets something a single 1,000 kVA machine cannot offer on its own: the ability to take one set out of service, run planned maintenance, and still keep power on the bus from the other. That is the main driver for most installations that carry synchronizing panels.

There is a second, quieter benefit. Load on an industrial site rarely sits at a fixed level through the day. A night shift or a weekend might need a third of the load a full production run needs. Paralleling lets a plant run only as many sets as the current load calls for, which keeps each engine loaded closer to its efficient band instead of one oversized machine idling at low output for most of its hours. Our guide to [generator sizing](/blog/generator-sizing-guide/) covers how this changes the sizing arithmetic compared with a single standby machine sized for peak load alone.

## The Conditions a Set Must Meet Before the Breaker Closes

Synchronising generators means matching four things on the incoming set to the running bus before the paralleling breaker is allowed to close. Close a breaker out of sync and the two sets fight each other through mechanical torque and current the instant the contacts touch, which is exactly the fault synchronization exists to prevent.

- **Voltage.** The incoming set's terminal voltage must match the bus voltage closely. A synchronizing relay or panel typically holds this to within a few per cent before permitting closure; the exact figure a given controller is set to should come from its configuration, not a guess.
- **Frequency.** The incoming set's frequency must be within a narrow band of the bus frequency, and it must be closing in rather than drifting apart, so that the two stay in step once connected.
- **Phase angle.** The three-phase voltage waveforms of the incoming set and the bus must line up in angle at the moment of closure. A synchroscope or a check-sync relay tracks this directly; closing at a large phase angle produces a current spike proportional to how far out of step the machines are.
- **Phase sequence.** The rotation direction of the phases (which conductor leads which) must match. This is checked once at commissioning and does not normally change afterwards unless wiring is disturbed, but it is worth confirming after any panel rewiring or cable replacement.

Manufacturer settings for exactly how tight these windows are configured vary by controller and by site, so the commissioning engineer's settings for the installed synchronizing relay govern, not a generic figure.

## Manual, Semi-Automatic and Fully Automatic Synchronizing

Three approaches to closing the paralleling breaker are common on industrial sites, and the difference is how much of the matching work is done by a person versus a controller.

Manual synchronizing puts an operator in front of a synchroscope, a set of voltmeters and frequency meters, adjusting the incoming engine's speed and the AVR's voltage trim by hand until the synchroscope needle is near the top and turning slowly, then closing the breaker at the right moment. It works, but it depends on the operator's judgement every time and leaves no record of how close the closure actually was.

Semi-automatic synchronizing (check synchronizing) lets an operator or the plant control system initiate closure, but a synchronizing relay checks that voltage, frequency and phase angle are within set limits and blocks the breaker if they are not. This is the common middle ground: a person decides when to try, the relay decides whether it is safe.

Fully automatic synchronizing lets the genset controller (common controllers on Nigerian sites include DSE and ComAp platforms) adjust the incoming engine's governor and the AVR itself to bring voltage and frequency into the matching window, then closes the breaker automatically once phase angle lines up, with no operator action beyond arming the sequence. This is standard on automatic mains failure and multi-set paralleling panels where sets must come on and off the bus without someone standing at the panel. See our post on [automatic transfer switch and AMF panels](/blog/automatic-transfer-switch-amf-panel/) for how this fits alongside mains-to-generator transfer logic on the same switchboard.

## Load Sharing Once the Breaker Closes

Closing the breaker only puts the incoming set on the bus at close to zero load. Sharing the running load between the paralleled sets is a separate function, and it happens in two planes: real power (kW), governed by the engine's speed governor, and reactive power (kVAr), governed by the alternator's AVR.

For kW sharing, most industrial paralleling uses droop governing. Each engine's governor is set to reduce speed slightly as its load increases, so that sets naturally settle at proportional load shares of the total kW demand without needing to communicate with each other. An isochronous scheme, or a load-sharing line between controllers, can hold frequency dead level and divide load by a defined ratio instead, which is more common where load steps are large and speed stability matters more than simplicity.

For kVAr sharing, AVR droop does the equivalent job on the reactive side. Without it, small differences between two AVRs mean one alternator tries to supply more reactive current than the other, and the surplus flows between the machines as circulating current rather than out to the load. That circulating current heats both alternators for no useful work and is one of the more common faults found on sites where AVR droop has been disabled or set incorrectly during a repair.

## Common Synchronizing and Paralleling Faults

The table below covers the faults that show up most often once a paralleling scheme is in service, as distinct from a first-commissioning problem.

| Symptom | Likely cause | What to check |
|---|---|---|
| Breaker will not close, sets never line up | Synchronizing relay limits set too tight, or governor/AVR trim range too narrow to reach the window | Relay setpoints against commissioning record; governor speed trim range |
| Incoming set trips on reverse power shortly after closing | Set closed with too little fuel/speed reference, ends up motored by the bus instead of supplying it | Governor speed bias at closure; reverse power relay setting and trip delay |
| Persistent circulating current between paralleled sets, alternators run hot | AVR droop compensation missing or mismatched between controllers | AVR droop wiring and setting on each set; current transformer polarity feeding the droop circuit |
| Load sharing uneven despite matching kVA ratings | Governor droop settings not matched between sets, or load-sharing line faulty | Droop percentage on each governor; continuity of the load-sharing interconnect |
| Voltage or frequency hunts once two sets are paralleled | Both AVRs or both governors fighting for isochronous control at the same time | Confirm only one set (or a dedicated master) runs isochronous; the rest run droop |
| Breaker trips on load transfer between mains and generator bus | Sync check relay not blocking closure outside its window, or contactor contacts worn | Sync relay function test; inspect and megger the breaker/contactor contacts |

## Commissioning and Testing a Synchronizing Panel

A synchronizing panel needs a defined commissioning sequence, not a single "it closed, so it works" trial. A reasonable sequence checks each function on its own before checking them together: verify phase sequence and rotation on each set individually, exercise the synchronizing relay's block function by deliberately running an engine outside its voltage or frequency window and confirming the breaker will not close, then close under normal conditions and record the closing transient on a data logger if the panel supports it.

Load sharing accuracy is tested by applying steps of load with the sets paralleled and confirming each set picks up its expected share within the governor's and AVR's droop settings, rather than only checking that the sets stay online. Our post on [generator load bank testing](/blog/generator-load-bank-testing/) covers how a load bank is used to apply controlled, repeatable load steps for exactly this kind of test, and it applies to a paralleled pair as much as to a single set.

Any work inside a synchronizing panel involves live low-voltage switchgear, and on larger sites the paralleling breaker itself may sit on medium-voltage gear. This work needs a qualified electrical engineer or technician working under lockout/tagout and a permit to work, not a description in an article substituting for that discipline.

Getting a synchronizing scheme right at commissioning, and keeping it right through the maintenance cycle that follows, is easiest to plan as part of a wider service contract rather than as a one-off panel job. Our [generator maintenance](/generator-maintenance-nigeria/) service covers governor and AVR checks, droop verification and synchronizing panel function tests as part of scheduled visits; where a fault has already appeared on a paralleled set, [request a technical proposal](/#contact) and we will scope the diagnostic work before quoting a fix.

## Frequently Asked Questions

### What is the difference between an ATS panel and a synchronizing panel?

An ATS or AMF panel transfers a load between two sources, typically mains and a generator, and only one source supplies the bus at a time during that transfer. A synchronizing panel closes two live sources onto the same bus at once, which needs the four sync conditions matched first. Some switchboards combine both functions where a site both transfers to generator power and paralleles multiple gensets.

### Can any generator controller synchronize with another set?

Only if the controller is designed and configured for paralleling, with the sensing, communication link (where fitted) and droop functions that paralleling requires. A standalone AMF controller running a single set typically lacks these functions even if the hardware looks similar. Check the controller's model and configuration against the manufacturer's paralleling documentation before assuming it can be paralleled.

### Why does a generator trip on reverse power right after synchronizing?

Reverse power means the set is being driven by the bus instead of supplying it, which happens when the incoming engine closes onto the bus without enough fuel or speed reference to immediately start carrying its share of load. The engine effectively idles while the alternator is spun by the other running set, and the reverse power relay (fitted to protect against this) trips it off. Correct governor speed bias at the moment of closure prevents it.

### How often should a synchronizing panel be tested?

There is no single interval that suits every installation, since it depends on how often the panel actually operates and the manufacturer's guidance for that controller. Sites that parallel daily exercise the synchronizing function constantly through normal operation; sites that rarely parallel should schedule a deliberate function test, including the block-on-out-of-window check, on a cycle set out in their maintenance contract or the panel manufacturer's manual.

### Does load sharing work the same way for gas gensets as for diesel?

The principle is the same: governor droop for kW sharing and AVR droop for kVAr sharing apply regardless of fuel. Gas engines can have narrower stable operating windows and different governor response characteristics than diesel engines, so droop settings tuned for a diesel set should not simply be copied onto a gas set without re-checking against that engine's governor response.
