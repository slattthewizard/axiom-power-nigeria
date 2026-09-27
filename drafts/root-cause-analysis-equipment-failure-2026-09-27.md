---
meta_title: "Root Cause Analysis for Plant Equipment Failure"
meta_description: "How root cause analysis finds the real cause of plant equipment failure in Nigeria: evidence, timeline, 5 whys, fishbone, fault tree and lasting actions."
primary_keyword: "root cause analysis"
secondary_keywords: "rca, 5 whys, fishbone diagram, fault tree analysis, equipment failure investigation"
---

# Root Cause Analysis for Plant Equipment Failure: A Practical Guide

A generator trips, a pump seal lets go, a turbine bearing runs hot, and the shift log fills up with a one-line entry: fault found, part replaced, unit returned to service. Three months later the same machine does the same thing. That is the gap root cause analysis is meant to close. It is the discipline of tracing a failure back past the part that broke to the reason it broke, so the fix addresses the actual problem and not just its most visible symptom.

For a plant manager or maintenance manager running equipment through Nigerian heat, dust and fuel variability, the temptation is always to swap the part and move on, because downtime has a cost attached to every hour. That instinct is sometimes correct for a genuinely random failure. But when the same failure mode keeps recurring across a fleet of generators, pumps or turbines, a proper RCA, done once, is usually cheaper than the third or fourth repeat repair.

This guide sets out how RCA should actually run: what to protect before anything else is touched, how to build a defensible timeline, which method (5 whys, fishbone diagram, fault tree analysis) fits which failure, and how to turn findings into actions that survive contact with a busy plant.

## What Root Cause Analysis Actually Delivers

Root cause analysis, often shortened to RCA, is a structured way of asking why a failure happened until the answer stops being another symptom and starts being something you can act on. "The bearing seized" is a symptom. "The bearing seized because oil supply to it was interrupted for 40 seconds during a controlled shutdown, and the interruption traced back to a check valve that had been sticking intermittently for weeks" is closer to a root cause, because it points at something specific to fix, monitor or redesign.

Done properly, RCA gives three things a bare repair report does not: a defensible account of what happened (useful for a warranty claim, an insurance question or a dispute with an operator), corrective actions ranked by what they actually prevent, and a record the next investigation on a similar asset can build on.

RCA is not a blame exercise, and treating it as one is the fastest way to get incomplete evidence and defensive answers from people who saw the failure happen. It is also not free: a thorough RCA takes real engineering hours, so it should be reserved for failures that are costly, safety related, or repeating, not every blown fuse.

## Preserving Evidence Before Anything Else Moves

The most common way a root cause analysis fails is that the evidence is gone before the investigation starts. A part gets thrown in the scrap bin, a control panel gets reset and its alarm history cleared, or the unit is already stripped for the replacement part by the time anyone asks what actually happened.

The moment a significant failure is identified, before repair work continues, four things are worth doing:

- Photograph the failed component and its surroundings from several angles before it is disturbed, including any debris, staining or fluid on nearby surfaces.
- Pull and record the controller or SCADA alarm history covering the hours before the trip, not just the trip itself. Many controllers hold only a limited buffer, so this should happen quickly.
- Tag and retain the failed part, along with any filters, oil or fuel samples taken near the time of failure, rather than sending them straight for disposal.
- Record who was present, the operating mode (load, ambient conditions, recent maintenance or setting change), and the exact alarm sequence as reported at the time, before memory fades or gets reshaped by later discussion.

Where the failure involves rotating machinery, pressurised systems or electrical isolation, that isolation and any lockout/tagout must be carried out by qualified personnel under a permit to work. Evidence gathering is never a reason to bypass isolation procedure.

## Building the Failure Timeline

Once evidence is secured, the next step is a timeline, and it should go back further than most first drafts do. A useful timeline spans three horizons: the minutes immediately before the trip (alarm sequence, load changes, operator action), the days and weeks before it (recent maintenance, parts changes, fuel deliveries, near-miss alarms reset without follow-up), and the months before it (last overhaul, condition monitoring trend, whether the asset has failed this way before).

A gas turbine trip, for example, is rarely explained by the trip signal alone. The investigation usually needs fuel gas quality trends, inlet air conditions, recent combustion adjustments and vibration trend data over a longer window; common trip causes worth checking first are covered in our piece on [gas turbine trip causes](/blog/gas-turbine-trip-causes/). The same logic applies to a pump seal or a [generator low-output](/blog/generator-low-output-causes/) event: the trigger is the last domino, not the first.

Building this timeline is easiest when the plant already logs routine readings, not just alarms. A site that only records data when something goes wrong will struggle to tell a genuine root cause from a plausible guess.

## Choosing a Method: 5 Whys, Fishbone, or Fault Tree

There is no single correct RCA method. The three used most often on industrial equipment differ mainly in how they handle complexity and how many contributing factors they are built to hold at once.

The 5 whys technique asks "why" repeatedly, using each answer as the basis for the next, until the chain reaches something actionable rather than another symptom. It suits a single, fairly linear failure chain and is quick to run with the people who were there. Its weakness is that a real failure often has more than one contributing branch, and a strict single-chain 5 whys can miss a second factor that was equally necessary.

A fishbone diagram (also called an Ishikawa diagram) organises possible causes into categories, commonly machine, method, material, manpower, measurement and environment, branching off a spine that points at the failure. It suits failures with several suspected contributing categories, but it is a brainstorming and organising tool, not a way of proving which branch actually caused the event.

Fault tree analysis works backwards from the failure using formal logic gates (AND, OR) to show which combinations of lower-level faults were necessary and sufficient to produce it. It suits safety-critical or repeat failures where two or more faults interact, such as a protection system that failed to trip because a sensor was reading incorrectly and a backup relay had also been left in test mode. It takes longer to build and is usually overkill for a single-cause failure.

| Method | Best suited to | What it produces | Main limitation |
|---|---|---|---|
| 5 Whys | Single, fairly linear failure chains | A short chain from symptom to root cause | Can miss a second contributing factor |
| Fishbone diagram | Failures with several suspected contributing categories | A structured map of candidate causes | Organises causes, does not itself prove which one |
| Fault tree analysis | Safety-critical or repeat failures with interacting faults | A logic tree showing which fault combinations were necessary | Takes longer to build, needs more data |

Many investigations use more than one in sequence: a fishbone to lay out candidate causes broadly, then 5 whys or a fault tree to work through the branches that survive scrutiny.

## Physical, Human and Latent Roots

A finding that stops at the physical cause, the part that actually failed, is usually only half the story. It helps to separate three layers.

The physical root is the mechanism of failure itself: a [bearing that ran without adequate lubrication](/blog/turbine-bearing-babbitt-failure/), a seal that ran dry, a winding that broke down from moisture ingress, a bolt that fatigued. This is generally the easiest layer to identify because it leaves physical evidence, provided that evidence was preserved.

The human root is the action or inaction that allowed the physical cause to develop: a lubrication round skipped under time pressure, a valve left in the wrong position after a shutdown, a setting changed without updating the reference documentation.

The latent root sits behind the human one and is usually the most valuable finding, because it is the one most likely to keep producing failures if left alone: a maintenance schedule with no time for the lubrication round to be done properly, a spares policy that meant the correct grade of oil was not on site so a substitute was used, a training gap that meant the operator did not know the setting mattered.

Take a hypothetical example: a 500 kVA standby generator suffers a turbocharger bearing failure. The physical root is oil starvation to the turbo bearing during a cold start. The human root is that the pre-start prime cycle was being bypassed to save time on a tight changeover window. The latent root is that the changeover procedure allows no time for a proper prime cycle, so the shortcut is built into the way the site operates the machine. Replacing the turbocharger fixes the physical failure. Fixing the changeover procedure stops it happening again on every set that follows the same routine.

## Turning Findings Into Actions That Stick

An RCA report that ends with "retrain staff" as its corrective action has usually stopped one step short of useful. Actions that hold up over time share three features: they are specific enough that someone could check whether they were done, they change something structural rather than relying on a person remembering to be careful, and they have an owner and a date attached.

"Improve lubrication discipline" is not a corrective action. "Add a mandatory prime-cycle interlock to the changeover sequence so the generator cannot accept load until oil pressure is confirmed, commissioned and tested by [date], owned by the maintenance planner" is. The first relies on human vigilance holding indefinitely. The second removes the opportunity for the shortcut to happen at all.

Rank actions by what they actually eliminate versus what they only reduce. An interlock that makes the failure physically impossible ranks above a procedure change that depends on compliance, which ranks above a reminder or training session, which tends to decay within months. Training still has value, but it should not be the only line in the action list for a failure that recurred because of a systemic gap.

A plant that wants root cause analysis to actually reduce downtime over time, rather than producing a paper trail after each event, generally needs it built into a wider audit of how the plant is run, not treated as a one-off exercise after a bad month. A structured [power plant audit](/power-plant-audit-nigeria/) looks at exactly this: whether the maintenance programme, spares stocking and operating procedures are set up to catch latent causes before they produce another failure, and whether corrective actions from previous RCAs were actually implemented. If you would like a second set of eyes on a recurring failure, [request a technical proposal](/#contact).

## Frequently Asked Questions

### How is root cause analysis different from a normal fault-finding report?

A fault-finding report usually stops at what failed and what was replaced. Root cause analysis asks why the failure condition developed and separates the physical failure from the human and organisational factors that allowed it. The output is a set of corrective actions, not just a repair record.

### Do we need a formal RCA for every equipment failure?

No. A structured RCA is worth the time for failures that are costly, safety related, or repeating. A one-off failure with an obvious, isolated cause can usually be closed out with a straightforward fault-finding note. Reserve the deeper methods for the failures that keep coming back or that carry real downtime cost.

### Which RCA method should a small maintenance team start with?

The 5 whys technique is the easiest to run without special training and works well for a single, fairly clear failure chain. Move to a fishbone diagram when several categories of cause are plausible, and reserve fault tree analysis for safety-critical systems or failures where more than one fault had to combine for the event to occur.

### Who should be involved in the investigation?

The people present at the time, the technicians who carried out the last maintenance on the asset, and someone with enough authority to commit to the corrective actions afterwards. Excluding operators for fear of blame usually produces a weaker investigation, because they often hold details that never reach the alarm log.

### What happens if the evidence has already been disposed of before the investigation starts?

The investigation can still proceed using the timeline, controller history and interviews, but the conclusions will carry more uncertainty and may not survive a warranty or insurance dispute. This is the main reason to fix evidence preservation as a standing instruction after any significant trip, rather than deciding case by case once the part is already gone.
