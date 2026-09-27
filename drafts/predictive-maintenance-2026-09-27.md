---
meta_title: "Condition Monitoring: Predictive Maintenance Techniques"
meta_description: "Condition monitoring techniques for Nigerian plants: vibration, oil, thermography and ultrasound, what each one catches, and where to start."
primary_keyword: "condition monitoring"
secondary_keywords: "condition based maintenance, vibration analysis, predictive maintenance techniques"
---

# Condition Monitoring and Predictive Maintenance Techniques for Industrial Plants

A bearing that fails on a Tuesday morning rarely fails without warning. It usually runs hotter, louder and rougher for weeks before it lets go, and on most Nigerian plants nobody is measuring any of those signs until the machine stops. Condition monitoring is the practice of measuring that early warning on purpose, on a schedule, so a failing bearing, seal or winding shows up as a trend on a chart rather than as an unplanned stop with production, a shift crew and a spare parts search all waiting on it.

This is not the same as preventive maintenance, which replaces parts on a fixed calendar whether they need it or not. Condition based maintenance measures the actual state of the equipment and acts on what the data shows. The two approaches work together rather than compete (see /blog/preventive-maintenance-plan/ for how a maintenance manager builds the calendar side), and most plants that get this right run a mix: fixed-interval tasks for consumables and safety-related items, condition monitoring for the rotating and electrical assets where failure is expensive and the warning signs are measurable.

This guide covers the techniques that make up a working condition monitoring programme on a Nigerian industrial site: vibration analysis, oil analysis, thermography, ultrasound and electrical signature analysis, what each one actually catches, and how a plant with no programme today should start.

## Vibration analysis: the first technique most plants adopt

Every rotating machine has a vibration signature, and that signature changes in a specific and often predictable way as a fault develops. An accelerometer mounted on a bearing housing picks up that signature, and software breaks it down by frequency so an analyst can separate imbalance, misalignment, bearing wear, looseness and gear mesh problems from each other rather than reading a single overall number.

The overall vibration level (a single figure summarising the whole signature) is useful as a screening tool and for trending against a machine's own history. Whether a given reading counts as acceptable, alert or alarm depends on the machine class, its mounting and its speed, and the applicable zone boundaries come from the OEM's own limits or the relevant ISO vibration severity tables for that machine class, not from a single number repeated across every asset on site. Where vibration is already high enough to be a symptom rather than a monitoring reading, /blog/steam-turbine-high-vibration/ covers the diagnostic route for a machine that is already showing a problem.

Vibration analysis is usually the first technique a plant adopts because the equipment is relatively affordable, the readings are quick to take on a walk-around route, and it catches a wide range of the failure modes that actually stop production: bearing defects, misalignment after a coupling job, unbalance after a fan blade builds up deposits, and looseness in a foundation or mounting that would otherwise go unnoticed until something breaks.

## Oil analysis: reading the machine through what it leaves behind

Lubricating and hydraulic oil carries evidence of what is happening inside a machine long before that machine shows an external symptom. A properly drawn oil sample, analysed for wear metals, contamination and the condition of the oil itself, tells an analyst whether a bearing or gear is shedding metal, whether water or process fluid has got into the system, and whether the oil itself still has useful life left or needs changing regardless of the calendar.

Wear metal analysis (typically by spectrometry) picks up the specific elements associated with different components: iron from steel gears and bearings, copper from bushings and some bearing overlays, aluminium from certain housings and pistons. A rising trend in one element, tracked sample to sample, points to which component is wearing before it reaches the point of a bearing failure with metal already audible through the casing. Contamination checks (particle count, water content, viscosity) catch the problems that damage a machine from the outside in: a failed seal letting in water or process gas, a filter bypassing, or a wrong oil topped up during a routine service. The full detail of what a lube oil analysis report actually measures and how to read a trend rather than a single result is covered in /blog/turbine-lube-oil-analysis/, and the same logic applies to reciprocating engines and gearboxes as it does to turbines.

## Thermography: seeing heat before it becomes a fault

An infrared camera turns surface temperature into an image, and on electrical and mechanical equipment, an unexpected hot spot is almost always a sign of a problem: a loose or corroded connection, an overloaded circuit, a failing bearing running hot, a blocked cooling passage, or insulation that has broken down enough to allow leakage current. Because the survey is done from a safe distance with the equipment running, it is one of the few techniques that finds a developing electrical fault without opening a live panel.

A useful thermography programme covers switchgear, busbar joints, transformer bushings, motor control centres and, on the mechanical side, bearing housings and coupling areas, on a fixed route so the same points get checked every time and a trend can be built rather than a single snapshot. A hot spot on switchgear or a live panel is a finding for a qualified electrician working under a permit to isolate and investigate, never a prompt to open a live enclosure to look closer: the camera exists precisely so nobody has to do that.

## Ultrasound: catching what the ear and the camera both miss

Airborne and structure-borne ultrasound detectors pick up high-frequency sound outside the range of human hearing, and on an industrial site that range is where two very different but very common problems both show up clearly: compressed air and gas leaks, and early-stage bearing defects.

A leak through a valve, fitting or hose produces a distinct rushing sound at ultrasonic frequency that an ultrasound gun can hear and pinpoint from several metres away, even in a noisy plant where a human ear would never isolate it from background noise. Regular ultrasound leak surveys on a compressed air system typically find a meaningful number of leaks that were previously invisible, and fixing them is one of the more direct energy savings available on a plant (see /blog/generator-sizing-guide/ for how compressor and other electrical load feeds into overall generator loading). On rotating equipment, a bearing developing surface defects produces a characteristic ultrasonic signature well before it shows up clearly in the audible vibration spectrum, which makes ultrasound a useful early-stage complement to vibration analysis rather than a replacement for it.

## Electrical signature analysis: reading the motor from its supply

Motor current signature analysis and related electrical techniques measure the current and voltage drawn by a motor and extract information about the mechanical condition of the equipment it drives, alongside the electrical health of the motor itself. A broken rotor bar, an eccentric air gap, a developing bearing fault, or a mechanical problem on the driven load (a pump impeller fouling, a fan blade imbalance) all leave a signature in the current waveform that a trained analyst can pick out.

The practical advantage on a Nigerian site is access: the measurement is taken at the motor control centre or starter, not at the machine itself, so a motor driving a pump in a pit, a fan on a roof, or equipment inside a hazardous area classification can be assessed without physical access to the machine. It is a specialist technique, usually brought in periodically rather than run as a continuous in-house programme, and it complements vibration and oil analysis rather than replacing either.

| Technique | What it mainly catches | Access needed |
|---|---|---|
| Vibration analysis | Bearing wear, misalignment, imbalance, looseness | Sensor on the machine, running |
| Oil analysis | Wear metal trends, contamination, oil degradation | Oil sample, machine running or just stopped |
| Thermography | Loose connections, overloads, cooling problems, hot bearings | Line of sight, no contact, running |
| Ultrasound | Air and gas leaks, early bearing defects, electrical discharge | Line of sight or contact, running |
| Electrical signature analysis | Rotor faults, mechanical faults transmitted through current | At the motor control centre, running |

## Starting small: which assets to put on a programme first

A plant with no condition monitoring today should not try to instrument everything at once. The starting point is a criticality list: which assets, if they failed unannounced, would stop production, create a safety event, or cost the most in downtime (see /blog/plant-downtime-cost-per-hour/ for how to put a figure on that cost). Large motors and pumps feeding a critical process line, generators and their prime movers, and any single machine with no installed spare typically sit at the top of that list.

For those assets, a basic route of vibration readings and, where relevant, an oil sample on a fixed schedule (monthly is common as a starting point, adjusted once a baseline exists) will surface most of the developing problems that matter. Thermography surveys of switchgear and motor control centres on a similar cycle cover the electrical side. A plant does not need every technique on every asset from day one: it needs the right technique on the assets where an unplanned failure actually hurts, with a baseline reading taken while the machine is healthy so later readings have something real to compare against.

## Common pitfalls that undermine a condition monitoring programme

The technology is rarely what makes a programme fail. The pattern that does is more mundane: readings get taken and filed without anyone reviewing the trend, alert thresholds are copied from a different machine class instead of set from the asset's own baseline, and a genuine warning sign gets logged but no work order follows because nobody owns the decision to act on it. A programme that generates data nobody reads is a cost with no benefit.

A second common failure is treating a single alarming reading as proof of an immediate fault rather than checking the trend and, where practical, taking a second reading before committing a machine to an unplanned outage. A one-off spike can come from a loose sensor, a temporary operating condition, or a measurement error, and reacting to every spike as a failure erodes confidence in the programme as fast as ignoring genuine warnings does. The techniques above work because they are trended and reviewed by someone who understands both the reading and the machine, not because a sensor was installed.

Building a criticality-ranked condition monitoring programme, or getting an independent read on where a plant's rotating equipment stands today, is scoped work rather than a fixed package: request a technical proposal through /#contact, or see the range of rotating equipment work this covers on /rotating-equipment-services-nigeria/.

## Frequently Asked Questions

### What is the difference between predictive maintenance and preventive maintenance?

Preventive maintenance replaces or services parts on a fixed calendar or running-hours interval regardless of their actual condition. Predictive maintenance, built on condition monitoring data, acts on the measured state of the equipment instead, which can mean running a component longer than a fixed interval would allow or catching a fault earlier than a calendar-based check would find it.

### Which condition monitoring technique should a plant start with?

Vibration analysis is usually the first technique adopted because the equipment cost is relatively low, readings are quick to collect on a walk-around route, and it catches a wide range of common rotating equipment failures. Oil analysis and thermography are typically added next, aimed first at the plant's most critical assets rather than everything at once.

### How often should vibration readings or oil samples be taken?

There is no single interval that applies to every plant. A monthly route is a common starting point for critical rotating equipment while a baseline is being built, then the interval is adjusted based on what the trend shows and the manufacturer's own guidance for that specific machine.

### Can condition monitoring be run entirely in-house?

Vibration route collection and basic thermography can be run by a trained in-house team once equipment and training are in place. Detailed vibration analysis, oil analysis interpretation and electrical signature analysis are more often brought in periodically as specialist services, since the value is in correct interpretation of the data rather than just collecting it.

### Does condition monitoring replace the need for planned outages and overhauls?

No. Condition monitoring changes when a planned outage or overhaul happens and what gets found once the machine is open, by giving advance warning of which components need attention. It does not remove the need for the outage itself on machinery that requires periodic internal inspection regardless of condition data.
