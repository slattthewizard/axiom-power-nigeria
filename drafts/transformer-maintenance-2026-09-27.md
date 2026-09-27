---
meta_title: "Transformer Maintenance Checklist for Nigerian Plants"
meta_description: "A practical transformer maintenance checklist for Nigerian plant engineers: oil tests, DGA, thermography, bushings, cooling and loading checks."
primary_keyword: "transformer maintenance"
secondary_keywords: "transformer oil test, transformer maintenance checklist, distribution transformer maintenance, dga"
---

# Distribution Transformer Maintenance: A Practical Checklist for Nigerian Plants

A distribution transformer rarely fails without warning. Oil turns dark, a bushing runs hot, a protection relay operates once and resets itself, and the signs sit in a test report weeks or months before the unit trips or bursts. For a factory, a refinery support facility, a hospital or a bank branch running its own step-down transformers, transformer maintenance is the difference between catching that pattern on a planned shutdown and losing the load, the transformer and the outage window all at once.

This article sets out what a working maintenance programme for a plant distribution transformer actually covers: oil sampling and the three core tests, dissolved gas analysis, thermography, bushing and cooling checks, and how to turn all of it into an interval schedule a maintenance team can follow. None of it replaces the OEM manual for the specific transformer on site, which governs on ratings, test values, clearances and tap settings.

Transformers get less attention than generators and turbines on most Nigerian sites, mainly because they sit quietly in a room or a yard and do not run out of fuel. That is exactly why they get missed until a fault forces a shutdown at the worst possible time.

## Why Plant Distribution Transformers Fail Early on Nigerian Sites

A few conditions repeat across factories, hospitals, telecom sites and bank branches:

- Ambient heat plus a poorly ventilated transformer room pushes winding and oil temperatures above what the nameplate assumes, shortening insulation life even when the load looks normal on paper.
- Dust and harmattan-season particulate load the cooling fins and clog breathers faster than the maintenance calendar expects.
- Frequent switching between grid and generator supply, especially around a grid collapse and restoration, exposes windings and bushings to voltage transients that a stable supply would not produce.
- Moisture ingress through a worn gasket or a saturated breather turns a healthy oil sample into a poor one over a single wet season.
- Many sites size their transformer for future load and then run it lightly loaded for years, which can mask an incipient fault because loading and temperature stay low.

None of this replaces a proper cause investigation on any specific unit. It is a starting list for where to look first.

## Oil Sampling and the Three Core Tests

Before dissolved gas analysis, a plant should have a routine on basic oil quality: breakdown voltage (BDV), moisture content and acidity (sometimes reported with interfacial tension). These three tests are quick, relatively cheap, and catch contamination and ageing long before a fault gas shows up.

IEC 60422 groups in-service mineral oil condition into good, fair and poor bands that vary with the transformer's voltage class, with lower voltage-class units (broadly under 72.5 kV, which covers most plant distribution transformers) generally expected to sit above roughly 30 to 40 kV BDV to be considered acceptable, and above roughly 40 kV to be called good. Moisture content limits tighten as the voltage class rises, because water in oil lowers the dielectric strength faster in a highly stressed insulation system. Treat these as typical bands from published guidance, not a substitute for the test lab's own report against the relevant standard, and always read the result against the oil type and the transformer's design temperature rise.

A rising acid number over successive samples, even while BDV still passes, is often the earliest sign that oil is oxidising and needs attention before it starts attacking paper insulation.

## Reading a Dissolved Gas Analysis Report

Dissolved gas analysis (DGA) looks at the specific gases that form when oil and cellulose insulation break down under heat or electrical stress, and it is the single most useful test for catching a developing transformer fault before it becomes an outage.

Hydrogen and methane in isolation usually point to a low-energy fault such as partial discharge. Ethylene rising alongside a general increase in gas usually points to overheating above roughly 300 degrees Celsius somewhere in the winding or connections. Acetylene is the gas that matters most: any meaningful acetylene reading points to arcing or a very high temperature fault, typically above 700 degrees Celsius, and is treated as urgent regardless of what the other gases show. Carbon monoxide and carbon dioxide track paper insulation degradation rather than the oil itself, and their ratio matters more than either figure on its own.

General screening limits published under IEEE C57.104 guidance for a mineral-oil transformer are commonly cited in the region of 100 ppm for hydrogen, 120 ppm for methane, 50 ppm for ethylene and 35 ppm for acetylene, with carbon monoxide guidance around 350 ppm, though the applicable table depends on the standard version and the transformer type. A single sample against these figures is a starting point. What actually predicts failure is the trend: how fast a gas is increasing between samples, rather than whether one number has crossed a line. A transformer with low absolute gas levels that are climbing quickly deserves more attention than one with a stable, higher baseline.

Do not try to interpret a DGA report from a template found online. Send it to a competent laboratory or engineer who will read the gas ratios, the rate of change and the transformer's history together.

## Thermography and Hot Connections

An infrared survey under normal load finds problems that oil and gas tests cannot: a loose cable lug, a corroded bolted connection, an unevenly loaded bushing, or a radiator bank that is not circulating oil because a valve was left shut after a previous outage.

The comparison that matters is relative: one phase or one connection running noticeably hotter than its equivalents on the same transformer, not an absolute temperature read off a thermal camera screen from a distance. Surveys should be done under a representative load, ideally close to peak demand for that circuit, and repeated on the same schedule so trends are visible year on year.

Thermography itself is a hands-off, non-contact test, but the survey often exposes a fault that then needs an energised connection opened, retorqued or replaced. That work involves live or recently isolated electrical equipment and must be carried out by qualified personnel under lockout/tagout and a permit to work, never by someone reading a thermal image and reaching for a spanner unsupervised.

## Bushings, Cooling and Loading Review

Bushings age differently from the oil in the main tank, and a bushing power factor (tan delta) test, done at the frequency the equipment class calls for, catches tracking, moisture ingress and internal deterioration that a visual check will miss. Oil level in oil-filled bushings should be checked against the sight glass at every routine visit.

Cooling should be reviewed against how the transformer is actually run rather than its nameplate alone: fans and pumps that cycle correctly, radiator fins free of dust and insect nests, and oil flow that is not restricted by a valve left in the wrong position. Loading review means checking actual demand history against the nameplate rating and the transformer's temperature rise class, because a unit bought for future expansion and then run near its rated capacity years earlier than planned will age its insulation faster than the same nameplate figure suggests on paper. A transformer originally specified as standby duty and now carrying continuous load needs its rating checked against how it is actually being used, in the same way a standby-rated generator does.

## Protection, Breather and Routine Checks

A few checks belong on every routine visit regardless of test cycle:

- Buchholz (gas and oil operated) relay: check for trapped gas, confirm alarm and trip contacts are wired and tested, and treat any accumulated gas as a sample to send for analysis, not something to bleed off and ignore.
- Pressure relief device: confirm it has not operated and is not leaking.
- Winding and oil temperature indicators: calibrate against a reference, since a drifting gauge either masks a real overheating trend or triggers nuisance alarms.
- Silica gel breather: a colour change from blue or orange toward pink or clear signals moisture has been absorbed and the desiccant needs regenerating or replacing, and a consistently saturated breather points to a seal or gasket problem worth chasing.
- Earthing and bonding continuity on the tank and neutral.

Any of this work that requires opening a control cubicle, testing a protection relay live, or accessing terminals still connected to source needs the same lockout/tagout discipline and permit to work as the bushing and connection work above.

## Building a Transformer Maintenance Interval Schedule

The table below is a typical cadence used across the industry for an oil-filled plant distribution transformer. Criticality, loading, environment and the OEM manual should all move individual tasks earlier or later than this starting point.

| Interval | Typical tasks |
|---|---|
| Daily to weekly | Visual check: oil level, leaks, breather colour, gauge readings, unusual noise or smell |
| Monthly to quarterly | Thermography under load; visual check of cooling fans, radiators and connections |
| Annually | Oil sampling (BDV, moisture, acidity) and DGA; protection relay function test; earthing check |
| Every 3 to 5 years or on condition | Bushing power factor/tan delta test; internal inspection where DGA or thermography flags a concern |

A programme built only around fixed calendar dates, with no room for a result that says "test again sooner", misses the point of running these tests in the first place. Treat every result as an input to the next interval, not a box ticked and filed.

A distribution transformer this important to a plant's uptime is a natural candidate for inclusion in a wider plant power audit rather than being tested in isolation. A [power plant audit](/power-plant-audit-nigeria/) looks at the transformer alongside the generators, switchgear and protection settings it interacts with, which is where most real-world transformer faults actually get caught early. Where a site wants a scoped assessment of its transformers and the rest of the electrical plant, [request a technical proposal](/#contact) rather than guessing at scope from a checklist.

Further reading on related maintenance disciplines: [turbine lube oil analysis](/blog/turbine-lube-oil-analysis/) covers the same fluid-testing logic applied to rotating equipment, [insulation resistance and megger testing](/blog/megger-test-insulation-resistance/) is the companion electrical test for motors and switchgear on the same site, [plant downtime cost per hour](/blog/plant-downtime-cost-per-hour/) sets out why an unplanned transformer outage costs more than the repair invoice, and a [generator maintenance contract](/blog/generator-maintenance-contract/) is worth reviewing as a model for how a transformer testing programme should be structured and reported.

## Frequently Asked Questions

### How often should a plant distribution transformer have an oil test in Nigeria?

Most programmes sample oil for breakdown voltage, moisture and acidity annually, with dissolved gas analysis run on the same schedule for transformers above a certain size or criticality. Heat, dust and frequent switching between grid and generator supply are reasons to shorten that interval rather than lengthen it, and the OEM manual for the specific unit should always be the final word on cadence.

### What does a dissolved gas analysis report actually tell an engineer?

It identifies which gases are forming inside the transformer as oil and paper insulation break down, and each gas or combination points toward a type of fault: low-energy discharge, overheating, or arcing. The rate at which gas levels are rising between samples matters more than a single reading against a limit table, so trending several samples over time gives a far more reliable picture than one result on its own.

### Can oil sampling and thermography be done while the transformer is still running?

Yes, both are designed to be carried out on a live, loaded transformer, which is part of why they are used so widely. Any follow-up work that finding triggers, such as tightening a hot connection or opening a bushing, is a different task that requires isolation, lockout/tagout and a permit to work carried out by qualified personnel.

### What is the biggest cause of early transformer failure on Nigerian industrial sites?

There is no single dominant cause, but moisture ingress through a saturated breather or a worn gasket, sustained overheating from a poorly ventilated transformer room, and voltage transients from repeated switching between grid and generator supply all show up repeatedly in practice. Most of these are catchable early by the routine checks and tests set out above rather than by any single test in isolation.

### Does a colour change in the silica gel breather mean the transformer has a serious problem?

Not on its own. A breather absorbing moisture and changing colour is doing its job, and regenerating or replacing the desiccant is routine maintenance. It becomes a concern only if the breather saturates unusually fast between visits, which points to a seal, gasket or ventilation issue that is letting in more moisture than the design expects, and that pattern is worth investigating rather than the single colour change itself.
