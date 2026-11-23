---
meta_title: "Generator Not Starting: Diagnosis for Standby Diesel Sets"
meta_description: "Generator not starting? Work through no crank, cranks but no start, and failed auto start on a standby diesel set, with a fault-finding sequence and table."
primary_keyword: "generator not starting"
secondary_keywords: "diesel generator not starting, generator cranks but will not start, generator not starting automatically, generator starting problems"
---

# Generator Not Starting: A Fault-Finding Guide for Industrial Standby Diesel Sets

A standby set that won't start is rarely a mystery once you ask the right first question: what does it actually do when you press start? Does it do nothing at all, does it turn over but never fire, or does it start fine by hand and then ignore a mains failure? Those are three different problems with three different lists of suspects, and mixing them up is how people end up changing a starter motor when the real fault is a dry fuel line.

This guide is written for plant and maintenance engineers looking after standby diesel sets, typically the kind that sit idle for weeks and are then expected to pick up the plant within seconds. The causes of a diesel generator not starting split cleanly by symptom, so that's how the article is organised. Work down the symptom you have, not the one you assume.

Honestly, most of these are fuel or battery problems. The expensive explanations, low compression or a failed injection pump, are real but they're the last things to blame.

## First, Decide Which of Three Problems You Have

Stand at the set, put the controller in manual and press start. Then sort what you see.

If the engine doesn't turn at all, or the starter clicks or whirs weakly, you have a no crank problem. The fault sits in the starting circuit: batteries, charger, starter, solenoid, or a controller that is refusing to start.

If the engine turns over at normal cranking speed for the full crank attempt but never fires, or fires briefly and dies, you have a cranks but no start problem. Cranking works, so the starting circuit is fine. The engine isn't getting fuel, isn't getting air, or isn't reaching compression.

If the set starts perfectly in manual but sits there when the mains drops, you have an automatic start problem. The engine is healthy and the fault is in the signal chain that is meant to ask it to start.

That one test saves hours. Before anything else, read the controller screen and log the alarm or status text. A latched fault will often name the problem directly, and our guide to [Deep Sea controller alarms](/blog/deep-sea-controller-alarms/) covers what the common ones mean.

## Safety Before You Touch Anything

A set that is not running isn't a set that is safe. It can start without warning from an auto start signal, the batteries can deliver very high fault current, and fuel and hot surfaces are present throughout. Before any hands-on work beyond reading the controller, put the controller in OFF, isolate the starting supply by disconnecting the battery negative, lock out the ATS or mains contactor, and apply lockout-tagout under a permit to work. Don't bleed fuel lines or crack injector pipes on an engine that could be cranked by someone else. Keep naked flames and cigarettes away from open fuel connections, and mop up spilled diesel before you leave the area.

## Group One: The Engine Won't Crank

When there's no rotation, start with the cheapest and most common cause and work outward.

**Batteries.** Standby sets spend most of their lives on float charge, and batteries that are flat, sulphated or simply old are the single most frequent reason for a no crank. A battery can show a healthy resting voltage and still collapse the moment the starter draws current. Check voltage at rest, then watch it on the controller while cranking. If it drops sharply, the battery has lost capacity, however good it looked a minute earlier. Loose, corroded or greasy terminals do the same job, so clean and tighten them with the battery disconnected before you condemn anything.

**Charger.** If the batteries are flat, ask why. A failed or tripped battery charger, a blown charger fuse or a lost AC supply to the charger will let a healthy battery bank run down over weeks without anyone noticing. Replacing the batteries without finding out why they died is a short-lived fix.

**Starter motor and solenoid.** A single loud click with no rotation points at the solenoid or at a poor connection on the starter feed. A starter that spins freely without engaging the flywheel suggests a worn Bendix drive or damaged flywheel teeth. A starter that turns slowly and sounds tired is more often a battery or cable problem than a failed motor. Voltage drop across the main starter cable under crank is a quick test of cable and connection condition.

**Controller in the wrong mode or holding a fault.** This catches people constantly. A controller left in OFF, or in a test or manual mode after the last service, will ignore start demands. A latched fault such as a previous overspeed, low oil pressure or emergency stop will also inhibit starting until it's cleared. Read the log first, fix whatever caused the shutdown, then reset.

**Emergency stop.** A pressed e-stop on the set, the control panel or a remote station will block starting. Check every one, including remote stations that a contractor may have pressed and forgotten.

## Group Two: It Cranks But Won't Start

This is where the diesel engine's own requirements matter. A diesel needs air, clean fuel at the right pressure, and enough compression to ignite it. Cranking speed is normally fine here, so look at what the engine isn't getting.

**No fuel at the engine.** Start with the plain things. Is there fuel in the tank, and does the gauge actually read true? Is the tank outlet valve open? A float-type gauge that sticks, or a day tank transfer pump that has stopped, will leave a set running dry while the main tank is full.

**Air in the fuel system.** This is the classic after a filter change or after the set has run out of fuel. Air in the lines stops the injection pump building pressure, so the engine cranks all day and never fires. Prime the system with the hand primer until the fuel runs bubble-free at the bleed points, then crank in short bursts. Cranking for long periods trying to pull fuel through will only drain the batteries and overheat the starter.

**Blocked filters.** Fuel filters clog with sediment, waxy residue and the sludge that builds up when diesel sits in a tank for months. The engine may start, run for a minute under no load and die, or refuse to start at all. A set that starts and then fades is a filter problem until proven otherwise.

**Fuel shut-off solenoid.** Most electronic and many mechanical sets use an energise-to-run or energise-to-stop solenoid on the injection pump. If it doesn't move, no fuel is delivered, whatever the controller does. Listen for the click when the start signal is given, check the supply voltage at the solenoid, and look for a failed solenoid or a broken wire.

**Contaminated fuel.** Water, microbial growth and sediment will block filters, corrode injection components and stop combustion. Standby tanks that are rarely turned over are particularly exposed. Draw a sample from the lowest point of the tank and look for water layers, haze and black slime. The damage this causes goes well beyond a failed start, and we've covered it in [contaminated diesel and what it does to a generator](/blog/contaminated-diesel-generator-damage/).

**Air intake restriction.** A badly blocked air filter, a stuck intake shutter left over from an overspeed shutdown, or a collapsed intake hose can starve the engine. It's less common than a fuel fault, but it takes thirty seconds to check.

**Low compression.** This sits at the bottom of the list on purpose. A worn engine with poor compression will crank freely and fail to start, often with white smoke and a rough cold start getting worse over time. A compression or cylinder leakage test will confirm it. Don't go there until fuel, air and the electrics are all cleared.

If the engine starts and then dies after a few seconds, look at the controller for a shutdown reason before you suspect fuel. Low oil pressure sensor faults and speed signal losses can both stop an engine that is mechanically fine.

## Group Three: It Won't Start Automatically on Mains Failure

If the engine starts every time in manual and fails only when the mains disappears, don't touch the engine. The fault sits in the logic between the mains sensing and the start command.

**Controller left in manual or off.** Automatic start only works with the controller in AUTO. After a service or a test, sets are left in manual more often than anyone admits. Make checking the mode part of the handover sign-off.

**AMF or ATS signal.** The mains failure signal has to reach the controller. A failed mains-sensing relay, a blown fuse in the voltage sensing circuit, a loose control wire or a faulty ATS auxiliary contact can all leave the controller convinced that the mains is healthy. Our guide to [automatic transfer switch and AMF panels](/blog/automatic-transfer-switch-amf-panel/) explains how that signal chain is built and where it breaks.

**Start delay and mains return settings.** Controllers have a start delay to ride through short dips. If it has been set too long, the set looks dead when it's just waiting. Check the start delay, the mains fail delay and the under- and over-voltage thresholds that define a failure, because a mains supply that is poor but not quite absent can sit inside the thresholds and never trigger a start.

**Remote start and failed inhibit signals.** On sets with remote start inputs, an inhibit signal, an external interlock or a wiring fault can stop an auto start that would otherwise run.

Test the whole chain on a scheduled basis. Opening the mains supply breaker under a permit to work and watching the set start and the load transfer tells you more than a manual start ever will.

## A Fault-Finding Sequence That Works

Following the same order each time stops you guessing. Check in this sequence, and don't skip ahead.

1. Read the controller. Record the mode, any active or latched alarm and the event log before you do anything that could clear it.
2. Check the obvious. Emergency stop released, controller in the right mode, fuel in the tank and the tank valve open.
3. Check the batteries under load, not at rest, and confirm the charger is working.
4. If it cranks, prime the fuel system, change or inspect the filters, and confirm the shut-off solenoid operates.
5. Sample the fuel from the bottom of the tank.
6. If it starts manually but not automatically, move to the mode, the mains sensing, the ATS signal and the delay settings.
7. Only after all of that, consider the starter, injection equipment and compression.

Take safety steps at every point where you reach into a panel or onto the engine: isolate, lock out and work under a permit.

## Quick Reference Table

| Symptom | Most likely cause | First check |
|---|---|---|
| No crank, nothing happens | Controller in OFF, latched fault or e-stop | Controller mode, alarm log, all e-stops |
| No crank, weak or slow | Flat or sulphated batteries, failed charger | Battery voltage during cranking, charger output |
| Single click, no rotation | Starter solenoid or poor connection | Voltage drop on the starter feed |
| Cranks, never fires | No fuel or air in fuel lines | Tank level, primer pump, bleed points |
| Starts, then dies | Blocked filters or fuel shut-off fault | Filter condition, solenoid supply |
| Cranks, white smoke, hard to start | Contaminated fuel or low compression | Tank sample, compression test |
| Starts in manual, not in auto | Controller in manual, ATS or AMF signal fault | Mode, mains sensing, start delay |

## Stopping It Happening Again

Almost every cause above is a maintenance cause. Load test the batteries and replace them on a schedule, drain water from the fuel tank and turn the fuel over, change filters on time, and run an on-load test that proves the automatic start chain. None of that costs anything like a plant outage. A set that is only ever run when the grid fails will always find the weakest point in your maintenance programme, usually at the worst moment. Our [generator maintenance](/generator-maintenance-nigeria/) service is built around exactly that: finding the starting faults on a planned visit rather than during a blackout.

If your set is already failing to start and you can't find the cause, or you want the starting system tested before the next outage, request a technical proposal through the [contact form](/#contact) and our engineers will arrange a site assessment.

## Frequently Asked Questions

### Why does my diesel generator crank but not start?

Because the starting circuit is working and something the engine needs for combustion is missing. The usual causes are no fuel at the injection pump, air in the fuel lines after a filter change or a dry tank, blocked filters, a fuel shut-off solenoid that isn't opening, or contaminated fuel. Low compression is possible on an old, worn engine but it's the last thing to suspect.

### Why does my generator click but not crank?

A single click usually means the starter solenoid is pulling in but the starter motor isn't turning. That points at a weak battery, a bad connection on the starter feed or a failing solenoid or starter. Measure battery voltage while cranking and check voltage drop across the starter cable before replacing parts.

### Why is my generator not starting automatically when the power goes off?

If it starts in manual, the engine is fine and the fault is in the auto start logic. Check that the controller is in AUTO, that the mains failure signal is reaching it, and that the start delay and voltage thresholds are set sensibly. A faulty mains sensing relay or ATS signal is a common cause.

### How often should I test a standby generator so it starts when needed?

A regular on-load test, commonly monthly, proves the starting circuit, fuel supply and transfer chain together, and the right interval depends on the set, its duty and the manufacturer's guidance. Include a full mains-fail test under a permit to work at planned intervals, not only a manual run.

### Can bad diesel stop a generator from starting?

Yes. Water, sediment and microbial growth block filters and can stop the injection system delivering fuel. Standby tanks that sit untouched for months are the most exposed, so sample from the bottom of the tank and treat or drain it before problems build up.
