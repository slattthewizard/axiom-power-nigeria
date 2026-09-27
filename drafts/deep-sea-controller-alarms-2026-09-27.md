---
meta_title: "Deep Sea Controller Alarms: What Genset Fault Codes Mean"
meta_description: "Deep Sea and ComAp genset alarms explained: low oil pressure, high coolant, fail to start, overspeed, and what to log before resetting in Nigeria."
primary_keyword: "deep sea controller"
secondary_keywords: "generator error codes, dse 7320 alarms, generator controller faults, comap controller"
---

# Deep Sea Controller Alarms and ComAp Fault Codes: What a Genset Panel Is Actually Telling You

A generator that has stopped mid-shift with a red light on the panel is not a mystery machine. It is a controller, most commonly a Deep Sea controller or a ComAp unit on industrial sets across Lagos, Port Harcourt and Abuja, reporting one specific condition it was built to catch. The trouble is that most sites clear the alarm and restart before anyone reads what it said, which is how a five-minute sensor fault turns into a seized engine two weeks later.

This is a working reference for plant, maintenance and facility managers on the alarms that show up most often on industrial diesel sets: low oil pressure, high coolant temperature, fail to start, overspeed, charge alternator failure and mains sensing faults. It covers what each one usually points to, what to record before anyone touches the reset button, and when resetting is the wrong move regardless of how urgent the load feels.

## How Deep Sea and ComAp controllers group their alarms

Deep Sea Electronics (DSE) modules such as the DSE7300 series, which includes the DSE 7320, and ComAp's InteliLite range are the two families a maintenance manager is most likely to meet on an industrial set in Nigeria. Both display live engine parameters on a back-lit screen and log events with a timestamp, and both split faults into two broad classes rather than treating every alarm the same way.

The first class is a warning: something is outside its normal band, but the set is allowed to keep running while someone investigates. The second is a shutdown, sometimes called an electrical trip on the ComAp range: the controller has decided the engine or alternator is at risk and stops the set immediately, whether or not the load cares. Deep Sea documentation for the 7300 series describes the module as continuously monitoring engine parameters and presenting warnings and shutdown information on its screen, and ComAp's InteliLite documentation uses shutdown ("Sd") and warning ("Wrn") prefixes on its own alarm list for the same reason. Knowing which class you are looking at tells you how much time you actually have before you decide what to do next.

## Low oil pressure

Low oil pressure is graded as a shutdown on both families because oil starvation destroys bearings and camshafts within seconds, not minutes. The controller reads it from a sender on the block, so the first question is always whether the engine truly lost pressure or the sender and its wiring failed instead. A genuine low reading after a cold start that settles once the engine warms up is different from a low reading that appears at load and stays.

Common causes on Nigerian industrial sites include a low sump level from an undetected leak, a clogged oil filter restricting flow, worn bearings reducing pressure at operating temperature, and a faulty pressure sender or a damaged wiring loop giving a false reading. Do not assume it is the sender until the dipstick and filter have been checked.

## High coolant temperature

A high coolant temperature shutdown is the engine telling the controller it is losing its ability to shed heat before something warps or cracks. On sites running long hours in Lagos or Port Harcourt heat, the usual suspects are a low coolant level, a radiator core blocked with dust (worse in the Harmattan season), a failed thermostat stuck shut, a slipping or seized fan belt, or a water pump that has lost its impeller vanes to cavitation or age.

Because a coolant alarm can follow a head gasket failure that is already letting combustion gas into the cooling system, do not simply top up and restart a set that has tripped on temperature more than once in a short period. Check the coolant for a diesel or exhaust smell and for oil contamination before returning it to service.

## Fail to start

A fail to start alarm means the controller ran through its cranking sequence, usually several attempts with a rest period between them, and never saw the engine reach a firing speed the controller recognises as running. This is different from an engine that starts and then trips on another alarm seconds later.

Work through it in order: confirm there is fuel reaching the injection system and that the tank is not simply empty or shut off at a valve, check starter battery voltage and terminal condition, confirm the fuel shut-off solenoid is energising, and rule out an engaged emergency stop or an open safety interlock somewhere in the start circuit. A set that cranks, fires briefly, then dies is usually a fuel or air problem, not a starting problem, and should not be treated the same way in the log.

## Overspeed

Overspeed is a shutdown on every controller worth trusting, and for good reason: an engine running away past its governed speed can shed a turbine blade, a flywheel component or worse in seconds. The controller reads speed from a magnetic pickup or from the alternator frequency, so an overspeed trip on a set that clearly never raced can point to a pickup fault, loose wiring, or a governor and actuator problem rather than a real runaway.

Because the consequence of getting this wrong is severe, an overspeed trip should always be treated as real until an engineer with the diagnostic tools to check actual engine speed says otherwise, never dismissed as "probably just the sensor" on the strength of a hunch.

## Charge alternator failure and mains sensing faults

A charge alternator failure alarm (sometimes shown as "charge alt fail" or similar) means the small belt-driven alternator that keeps the starting battery topped up while the engine runs is not producing output. It will not stop the set immediately in most configurations, but ignore it for long enough and the battery runs down, which shows up later as a fail to start on a set that was working fine the day before. Causes range from a snapped or slipping belt to a failed alternator or a blown fuse in the charging circuit.

Mains sensing faults sit on the AMF (auto mains failure) side of the controller rather than the engine side: the module has detected the incoming grid supply is outside acceptable voltage, frequency or phase parameters and has acted on it, either starting the set or blocking a transfer depending on how the panel is configured. This is the same logic that runs inside an automatic transfer switch panel, and a mains sensing fault that will not clear even when the grid looks fine on a meter is often a sensing input, contactor or panel wiring issue rather than a genuine supply problem. Our guide to [automatic transfer switch and AMF panels](/blog/automatic-transfer-switch-amf-panel/) covers how that side of the system is meant to behave.

## Alarm summary table

| Alarm | Class | Usually points to first |
|---|---|---|
| Low oil pressure | Shutdown | Sump level, filter, sender/wiring, worn bearings |
| High coolant temperature | Shutdown | Coolant level, radiator blockage, thermostat, belt, water pump |
| Fail to start | Lockout after cranking | Fuel supply, battery/starter, solenoid, interlocks |
| Overspeed | Shutdown | Speed pickup/wiring first, governor and actuator if pickup is sound |
| Charge alternator failure | Warning | Belt condition, alternator output, charging circuit fuse |
| Mains sensing fault | AMF-side alarm | Sensing input, contactor, ATS/AMF panel wiring |

## What to log before anyone resets the panel

The reset button on a Deep Sea controller or a ComAp unit clears the alarm from the screen. It does not fix anything, and once cleared, some of the evidence that would have told an engineer what actually happened is gone with it. Before resetting, write down the exact alarm text or code shown, the engine hours at the point of the trip, the readings on the screen for oil pressure, coolant temperature and battery voltage at that moment, and anything unusual in the seconds before the trip, such as a load step or a smell.

Do not reset and restart a set that tripped on low oil pressure or high coolant temperature until the underlying cause has been checked and confirmed clear. Restarting an engine that lost oil pressure for a real mechanical reason, rather than a sensor fault, can finish off bearings that a shutdown alarm was trying to protect. The same caution applies to an overspeed trip: confirm actual engine speed behaviour before assuming it is safe to bring the set back up.

Any investigation into wiring at the controller, the AMF panel or the alternator terminals is electrical work and needs a qualified technician working under lockout/tagout and a permit to work, not a machine operator guessing with a multimeter on a live panel. The same applies to any check inside a rotating machine enclosure while the set could restart automatically under an AMF sequence.

If alarms are recurring on the same set, or a fault report needs to go beyond "reset and it ran fine," that is the point to bring in a structured fault diagnosis rather than repeated resets. Our team can [request a technical proposal](/#contact) for a plant assessment covering controller logs, sensor calibration and the mechanical checks behind the alarm, or you can start from the broader [industrial generator and genset maintenance](/generator-maintenance-nigeria/) service page for what a scheduled programme covers.

## Frequently Asked Questions

### What does DSE stand for on a generator controller?

DSE stands for Deep Sea Electronics, a UK-based manufacturer of auto-start and auto mains failure control modules used widely on industrial and commercial gensets, including the DSE7300 series referenced in this article. The module handles starting, monitoring, protection and, on AMF-configured panels, automatic transfer logic.

### Is a warning alarm safe to ignore until the next service?

No. A warning means the controller judged the condition survivable in the short term, not that it is unimportant. Charge alternator failure and similar warnings tend to compound quietly, such as a flat starting battery weeks later, so they should be logged and investigated at the next planned stop rather than left until the next scheduled service.

### Why does my generator keep tripping on the same alarm after I reset it?

A repeat trip on the same alarm almost always means the underlying condition was never resolved, only cleared from the screen. Continuing to reset and restart risks running the fault to failure. Treat a repeat trip as a signal to stop and investigate rather than a nuisance to clear again.

### Can a faulty sensor cause a false shutdown alarm?

Yes, and it happens often enough that checking the sender and its wiring is a normal first step, particularly for oil pressure and speed pickup faults. That said, a genuine mechanical fault can present with exactly the same symptoms, which is why the underlying cause should be confirmed rather than assumed before restarting.

### Do ComAp controllers use the same alarm categories as Deep Sea controllers?

Broadly, yes. ComAp's InteliLite range uses shutdown and warning categories in the same spirit as the Deep Sea 7300 series, even though the exact labels, codes and screen layout differ between manufacturers. The engineering logic behind low oil pressure, high coolant temperature, overspeed and fail to start alarms is the same regardless of which brand of panel is fitted.
