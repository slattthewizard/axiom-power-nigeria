---
meta_title: "Gas Turbine Trip Causes: Spread, Vibration, Flame-Out"
meta_description: "Gas turbine trip causes explained: how exhaust spread, vibration and flame-out signatures point to the real fault before you open the machine in Nigeria."
primary_keyword: "gas turbine trip causes"
secondary_keywords: "gas turbine tripping under load, exhaust temperature spread alarm, gas turbine flame-out, turbine vibration trip, gas turbine troubleshooting Nigeria"
---

# Gas Turbine Trip Causes: Reading Exhaust Spread, Vibration and Flame-Out Signatures

A 5.5 MW gas turbine trips at 14:20 on a Tuesday, the plant swings onto diesel, and before the week is out the fuel bill for that single event has passed NGN 50 million (about USD 32,000) without anyone opening a casing. That is the real arithmetic behind gas turbine trip causes. The machine is rarely the expensive part of the problem. The guessing is.

Most units we are asked to look at have already had two or three components changed on suspicion, and they are still tripping. Thermocouple sets get replaced because the spread alarm mentioned temperature. Rotors get quoted for balancing because the vibration number was high. Neither decision was wrong on its face, but neither was supported by the data the machine handed over in the sixty seconds before it came off load.

A trip is not a failure. It is a protection function doing what it was set to do, and it leaves a signature behind. Read the signature properly and you usually know the fault class before the borescope goes in.

USD equivalents below are shown at roughly NGN 1,550 to the dollar. Check the rate on the day you build your budget, and treat every cost band as indicative until a survey has been done on your machine.

## The First Hour After a Trip Decides What You Can Learn

The most common failure in trip investigation in Nigeria is not technical. It is that the unit is restarted before anyone captures the data, and the evidence is gone.

Four things need pulling before the restart. The first-out annunciation, which tells you which protection actually operated rather than which alarms followed. The process trend at one second resolution for at least sixty seconds before the trip. The full exhaust thermocouple array, channel by channel, not the averaged value on the overview screen. And the vibration channels with their phase reference, if the machine carries proximity probes rather than casing seismic pickups only.

Here is the practical trap. Many turbine control systems on Nigerian sites historise at one minute averages, sometimes with deadband compression on top. A spread event that opened over ninety seconds shows up as a single flat sample. You cannot diagnose what the historian never recorded, so the first corrective action on some sites is a historian configuration change, not a mechanical one.

If your unit has tripped more than twice this quarter and nobody has pulled the second by second record, that is where the work starts. [Request a technical proposal](/#contact) or call [+234 803 000 0000](tel:+2348030000000) and an engineer will go through the trip log and the control configuration with you before anything is quoted.

## Exhaust Temperature Spread: The Most Readable of All Gas Turbine Trip Causes

Spread is the difference between the highest and lowest thermocouple in the exhaust array. On a can-annular machine each thermocouple sees gas that has swirled a predictable number of degrees around the annulus from a specific combustion can. That relationship is what makes spread diagnostic rather than merely alarming.

Two low channels sitting at a fixed circumferential offset, with the offset matching the machine's swirl characteristic, points at one can: a coked fuel nozzle, a cracked transition piece, a distorted liner. One low channel with no partner, appearing as a step change rather than a ramp, is far more often an instrument fault such as an open thermocouple circuit, a corroded extension junction box or a cold junction compensation error.

Timing matters as much as pattern. Spread that is acceptable at idle and opens as you load usually means a fuel distribution problem that only shows at higher fuel flow. Spread present from light-off is more often instrumentation, or a can that did not light cleanly.

Be honest about the limits. Mapping a thermocouple back to a specific can needs the swirl chart for your exact machine and exhaust arrangement. Without it the pattern still separates instrument from combustion, but not which can, and you are into a full borescope rather than a targeted one.

**A flour mill west of Lagos.** A wheat mill on an industrial estate outside Lagos ran a 5.5 MW can-annular unit on a captive scheme. It tripped on high exhaust spread four times in three weeks, always between 40 and 70 percent load during the afternoon ramp. The site had already replaced the complete thermocouple set at NGN 3,200,000 (about USD 2,065) and the trips continued.

The one second data told a different story. Spread opened from 22 K to 61 K over roughly ninety seconds each time, which is a ramp, not the step an instrument failure produces, and two low channels sat at a consistent offset. Borescope inspection found heavy coking on one fuel nozzle and a failed transition piece seal on the adjacent can.

Combustion inspection with nozzle refurbishment and seal replacement came to NGN 26,400,000 (about USD 17,000) over a six day outage. The four unplanned trips had already burned roughly NGN 54,000,000 (about USD 34,800) in AGO covering a 3.2 MW load on standby diesel. The repair cost less than the trips that preceded it, and the mill scheduled the outage into an existing gap in wheat deliveries to hold the diesel exposure down.

## Vibration Trips: Amplitude Alone Tells You Almost Nothing

A vibration trip gives you one number on the panel and that number is close to useless on its own. What you need is frequency content, phase, direction and the trend of change.

The broad reading works like this. A rise at running speed with a phase shift usually points to unbalance from deposits, blade damage or a developing rub. A strong second order component with an axial contribution points at misalignment or a coupling fault. Sub-synchronous activity around 0.4 to 0.5 times running speed suggests an oil film instability in a journal bearing. Broadband high frequency energy points at rolling element bearings or blade contact.

Whether the trip happens on run-up through a critical speed or at steady load narrows the field further. Thermal bow and rotor rubs behave nothing like a foundation fault.

Evaluation criteria for machine vibration are set out in [ISO 20816-1](https://www.iso.org/standard/63180.html), which covers measurement position, magnitude zones and, importantly, evaluation of change rather than absolute level. The zone boundaries are general guidance. Your machine's own alarm and trip settings, fixed by the OEM against that rotor and bearing design, are what govern.

**A processing plant in Rivers State.** An 11 MW unit tripped on high vibration at 11.2 mm/s during run-up after a routine shutdown, three attempts running. The obvious reading was rotor unbalance, and a rotor removal and balance scope had been quoted at NGN 96,000,000 (about USD 62,000) with a long lead time on the balancing slot.

Phase referenced data said otherwise. The dominant component was at twice running speed with roughly 180 degrees of phase difference across the coupling and a clear axial component, which is a misalignment signature. Cold alignment checked within tolerance. Hot alignment did not, because two soleplate shims had gone missing during an earlier bearing job and the grout under one pedestal had softened.

Grout repair, re-shimming and hot alignment correction came to NGN 8,900,000 (about USD 5,700) over four days. Work of this kind sits under our [rotating equipment services](/rotating-equipment-services-nigeria/) scope and needs proper instrumentation and a qualified engineer on site. It is not a job for a straight edge and feeler gauges on a machine of this size.

## Flame-Out: Separating a Real Loss of Flame From a Detection Fault

A flame-out trip is one of the few where the signature settles the question quickly, provided you have the exhaust temperature trend at usable resolution.

If flame detection is lost and exhaust temperature collapses immediately behind it, the flame really went out. If detection is lost while exhaust temperature holds steady for several seconds, you are looking at a detection problem: a fouled scanner lens, a blocked sight tube purge, or a scanner drifted out of sighting alignment.

Genuine flame-out on gas fired machines usually traces to the fuel side. A supply pressure dip at the skid inlet during an upstream compressor cycle. Liquid carryback from a knock-out drum that has stopped draining. Gas composition drift, which changes the Wobbe index and therefore the heat release for a given valve position. Sudden load rejection also throws the combustor into a transient it may not ride through, depending on control response.

Fuel composition and dew point cannot be diagnosed from control screens. It takes a gas sample analysed against the machine's fuel specification, and if the gas comes through a local supplier rather than a major pipeline, that analysis is worth doing before spending anything on the turbine.

One safety point stated plainly. Purge credit, relight logic and the number of permitted restart attempts are protection settings governed by the OEM sequence and by combustion safety codes such as NFPA 85. They are not operator adjustments and should not be relaxed to get a unit back on load faster. If a machine will not relight, the correct response is a diagnosis, not a bypass.

If combustion behaviour has changed since a fuel supply switch, [book a plant assessment](/#contact) and have the fuel, the skid and the control response examined together rather than in isolation.

## Trip Causes That Sit Outside the Turbine Entirely

A large share of trips have nothing to do with the hot section. They come from auxiliaries, from protection settings, or from the network the generator is tied to.

The usual auxiliary suspects are lube oil low pressure from a failing pump changeover or a clogging filter, cooling water flow loss, instrument air loss on a pneumatically actuated fuel valve, and low DC supply to the trip circuit from a battery bank nobody has load tested in two years. Each presents as a turbine trip on the panel. None of them is a turbine fault.

Then there is the grid. Plants running in parallel with the network see undervoltage, underfrequency and reverse power events that operate generator protection correctly. Disturbances are frequent enough in Nigeria that the real question is whether relay settings match the plant's intended ride-through and the terms of its interconnection or captive arrangement, which sits under the framework administered by the [Nigerian Electricity Regulatory Commission](https://nerc.gov.ng/). Relay event records and disturbance recorder data settle this in an afternoon.

Ambient conditions matter more than most operators allow for. A gas turbine loses output roughly 0.5 to 0.9 percent for each degree C of inlet air temperature above ISO conditions, depending on the machine, and compressor fouling stacks on top of that.

**A bottling plant in Kano.** A beverage plant found its unit tripping on high exhaust temperature between December and February at loads it had carried comfortably in September. Filter differential pressure had climbed from 0.6 kPa to 1.9 kPa, and while on-line washes were being done, the off-line crank wash had been skipped for fourteen months.

An off-line wash over a ten hour window plus a filter element change came to NGN 4,300,000 (about USD 2,770) and recovered most of the lost output. Not all of it. Some fouling is not water soluble and only comes off at a compressor inspection, and no amount of washing removes the ambient derate. The seasonal pattern is covered in our note on [harmattan dust and turbine derating](/blog/harmattan-dust-turbine-derating/).

## What Gas Turbine Trips Cost to Diagnose and Correct

The table groups the signatures above against likely cause class, first diagnostic step and an indicative cost band. Treat the bands as planning figures for a proposal conversation, not as a quotation.

| Trip signature | Likely cause class | First diagnostic step | Cost band (NGN) | USD equivalent |
| --- | --- | --- | --- | --- |
| Spread ramps with load, two low channels at fixed offset | Fuel nozzle fouling or transition piece damage on one can | Targeted borescope, nozzle flow check | 4,500,000 to 38,000,000 | 2,900 to 24,500 |
| Spread steps on one channel only | Thermocouple, extension wire or cold junction fault | Loop resistance and cold junction verification | 900,000 to 4,500,000 | 580 to 2,900 |
| Running speed vibration rise with phase shift | Deposit unbalance, blade damage or developing rub | Phase referenced survey, off-line wash trial | 2,500,000 to 45,000,000 | 1,600 to 29,000 |
| Twice running speed with axial component | Misalignment, soft foot, foundation or grout failure | Cold and hot laser alignment, foundation check | 3,500,000 to 12,000,000 | 2,250 to 7,700 |
| Flame loss with exhaust temperature collapse | Fuel pressure dip, liquid carryover, composition drift | One second fuel pressure trend, gas analysis and dew point | 6,000,000 to 55,000,000 | 3,900 to 35,500 |
| Flame loss with exhaust temperature holding | Flame scanner fouling, purge blockage or sighting | Scanner clean, sight tube purge verification | 700,000 to 3,000,000 | 450 to 1,950 |
| Trip coincident with a network event | Protection setting or genuine grid disturbance | Relay event record and disturbance recorder review | 1,200,000 to 8,000,000 | 780 to 5,200 |

Two things stand out. The cheapest rows are the instrument and protection ones, and those are exactly the faults most often misdiagnosed as hot section damage. The expensive rows are expensive mainly because of the outage window they need, not the parts.

That is the calculation to put in front of your management. A combustion inspection you schedule is a cost you control. The same work forced on you by a fifth trip costs the same plus whatever your diesel cover burns, and the standby fleet ages faster while it carries the load. Where the money goes across turbine and generator work is set out under [turbine and generator maintenance cost](/generator-turbine-maintenance-cost/), and the point at which a machine has passed economic repair is covered in [overhaul versus replacement](/blog/turbine-overhaul-vs-replacement/).

The last piece is a trip register. One row per event with date, load, ambient, first-out annunciation, spread at trip, vibration at trip and what was done. After six entries the pattern is usually visible without any extra instrumentation, and it is the most useful document you can hand an engineer at the start of a survey. Inspection frequency should also be reviewed against [turbine inspection intervals](/blog/turbine-inspection-intervals/) once a unit starts cycling on trips, because run hours alone stop being a fair measure.

If you want the trip history read properly before the next outage is planned, [request a technical proposal](/#contact) or speak to an engineer on [+234 803 000 0000](tel:+2348030000000). We scope the diagnosis first and quote the correction afterwards, in writing, against what the data shows. Where the work touches the steam side of a combined arrangement, it sits under [steam and gas turbine overhaul](/steam-turbine-overhaul-nigeria/).

## Frequently Asked Questions

### What is the most common cause of a gas turbine trip?

Across the machines we are called to, instrument and auxiliary faults are more common than hot section damage, though they are diagnosed less often. Thermocouple failures, lube oil pressure switches, instrument air and protection relay settings account for a large share of trips initially assumed to be combustion problems. The honest answer still depends on your machine, its fuel, its duty and its maintenance history, which is why data capture comes before diagnosis.

### Can we restart the turbine straight after a trip?

Not before the data is captured, and not until you know which protection operated and why. Restarting clears the fast trend buffers on many control systems and destroys the evidence that would have shortened the investigation. Repeated restart attempts after a flame-out also carry a real combustion risk, and the permitted number of attempts is set in the OEM sequence for a reason.

### How do we tell a thermocouple fault from a genuine combustion fault?

Look at the shape of the change and the company the channel keeps. An instrument fault typically appears as a step on a single channel with no matching partner in the array, while a combustion fault appears as a ramp, usually involving channels at a consistent circumferential offset. Loop resistance and cold junction checks confirm the instrument case in under an hour, which makes it the cheapest test to run first.

### Does harmattan dust actually cause trips, or only lower output?

Both, through the same mechanism. Compressor fouling reduces air flow and compressor efficiency, so the machine needs a higher firing temperature to hold the same load, and eventually the exhaust temperature control curve or the trip setting is reached. Washing recovers a good part of it, but not all fouling is water soluble and the ambient derate cannot be washed away, so some seasonal load planning is unavoidable.
