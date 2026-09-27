---
meta_title: "How a Gas Turbine Works: Industrial Guide for Nigeria"
meta_description: "A plain guide to how an industrial gas turbine works, its main parts, and what degrades performance at gas fired plants in Nigeria."
primary_keyword: "gas turbine"
secondary_keywords: "gas turbine working principle, gas turbine parts, how does a gas turbine work, industrial gas turbine"
---

# How Does a Gas Turbine Work? A Plant Engineer's Guide for Nigeria

A gas turbine trip in the middle of a production run raises the same first question every time: what actually goes on inside that machine between the fuel gas skid and the generator terminals. Plant managers and maintenance engineers running gas fired IPPs, refinery utilities or large factory power islands do not need a physics lecture, but a working grasp of the gas turbine working principle makes it far easier to read alarm logs, question a service report and plan an outage properly.

This guide sets out how an industrial gas turbine actually works, section by section, then covers the practical part: how heavy-duty and aeroderivative machines differ, and what tends to wear them down faster in Nigerian conditions than in a Gulf coast or European site with cleaner intake air and steadier fuel gas quality.

None of this replaces the OEM operation and maintenance manual for a specific frame. It is a reference point for reading that manual with more understanding, and for asking a service provider sharper questions before an overhaul or a major inspection.

## The Brayton cycle in plain terms

Every industrial gas turbine, whatever the frame or manufacturer, runs on the same thermodynamic cycle: the Brayton cycle. Air is drawn in, compressed, heated by burning fuel, and expanded through a turbine section that extracts work from the hot, high pressure gas. Part of that work drives the compressor itself; the rest is available at the output shaft to turn a generator, or in mechanical drive applications, a compressor or pump train.

Three things happen to the working fluid, in sequence:

- Compression: ambient air is compressed through a multi-stage axial compressor, raising its pressure and temperature before combustion.
- Combustion: fuel is added in the combustor and burned at close to constant pressure, sharply raising the gas temperature.
- Expansion: the hot gas expands through the turbine section, dropping in temperature and pressure while doing work on the rotor.

Unlike a diesel or gas reciprocating engine, none of this happens in discrete strokes. Compression, combustion and expansion run continuously and simultaneously in different sections of the same machine, which is why a gas turbine has so few reciprocating parts and why its condition depends so heavily on clean, steady airflow and consistent fuel gas quality rather than on piston rings and bearings in the way a diesel genset does.

## The main sections of an industrial gas turbine

Strip away the casing and auxiliary systems and an industrial gas turbine has four functional sections.

The air inlet and compressor take in filtered ambient air and raise its pressure, typically by a factor in the range OEM compressor maps quote for that specific frame, through a series of rotating and stationary blade rows. Compressor blade condition and inlet filtration quality set a hard ceiling on how efficiently the whole machine can run, because every percentage point of compressor efficiency lost to fouling or blade damage has to be made up somewhere else in the cycle.

The combustor mixes compressed air with fuel gas (or liquid fuel on dual-fuel units) and burns it in one or more combustion chambers, or in an annular combustor arrangement on many modern frames. Combustor liner condition and fuel nozzle cleanliness directly affect firing temperature uniformity, which in turn affects hot section life.

The turbine section extracts energy from the hot combustion gas across several stages of rotating blades and stationary vanes, converting thermal and pressure energy into shaft work. This is the hot gas path, and it is where the highest temperatures and the most expensive metallurgy in the machine are found.

Auxiliary systems keep the core running: lube oil systems for bearings, cooling and sealing air paths drawn off the compressor, fuel gas conditioning skids, vibration and temperature monitoring instrumentation, and the starting system, whether that is a static frequency converter, a diesel starter motor or, on smaller units, an electric motor. A trip on any one of these support systems shuts the whole unit down even though the core gas path may be completely healthy, which is one reason a proper fault log matters before anyone assumes the turbine itself has failed. For the common failure signatures behind an unplanned shutdown, see /blog/gas-turbine-trip-causes/.

## Heavy-duty versus aeroderivative gas turbines

Industrial sites in Nigeria run both families, and the choice affects almost everything about how the unit is operated and maintained.

Heavy-duty (also called industrial frame) gas turbines are built as a single, heavy casing designed for long continuous runs, with a thicker rotor and casing that tolerate slower starts and more frequent fuel quality variation. They dominate baseload power generation and large gas-to-power IPPs.

Aeroderivative gas turbines are adapted from aircraft engine cores paired with an industrial power turbine. They are lighter, start and reach full load much faster, and generally reach higher simple-cycle efficiency at a given size, which suits peaking duty, standby generation for critical loads, and mechanical drive duty on compressor trains where fast, reliable starts matter more than absolute robustness to fuel variation.

| Characteristic | Heavy-duty (industrial frame) | Aeroderivative |
|---|---|---|
| Typical duty | Baseload, continuous running | Peaking, standby, mechanical drive |
| Start time | Slower, minutes to tens of minutes | Fast, often under 10 minutes to full load |
| Fuel flexibility | Generally more tolerant of fuel gas variation | More sensitive to fuel gas quality and moisture |
| Maintenance approach | Scheduled major inspections tied to fired hours and starts | Modular, engine-core exchange or on-site module swap |
| Footprint and weight | Heavier casing, larger footprint | Compact, lighter, easier to transport |

Neither family is inherently better; the right choice depends on load profile, fuel supply reliability and how the unit sits in the wider power or process system. For a broader look at how gas turbines fit against combined cycle and simple cycle configurations, see /blog/simple-cycle-vs-combined-cycle/.

## What degrades a gas turbine faster in Nigerian conditions

The physics of the Brayton cycle does not change with geography, but the two inputs that drive it, inlet air and fuel gas, are harder to keep clean and consistent on many Nigerian sites than the OEM datasheet assumes.

Inlet air quality is the first issue. Harmattan dust loads the compressor inlet filters and, once filtration is overwhelmed or poorly maintained, fouls compressor blading, dropping compressor efficiency and pushing firing temperature up for the same output. Coastal sites in Lagos, Port Harcourt and Warri carry salt-laden air instead, which brings its own fouling and corrosion risk on compressor blading if filtration and blade coatings are not matched to a marine environment. The seasonal derating this causes is covered in more detail at /blog/harmattan-dust-turbine-derating/.

Fuel gas quality is the second. Pipeline gas composition, moisture content and the presence of liquids or particulates vary more on associated and non-associated gas supply in parts of the Niger Delta than a machine designed against a clean pipeline gas specification expects. Wet or dirty fuel gas damages fuel nozzles and combustor hardware, and in more severe cases can carry liquids into the hot gas path. A fuel gas conditioning skid sized and maintained for the actual gas being delivered, not the gas specification on paper, is one of the more overlooked protections on Nigerian gas-fired sites.

Grid instability adds a third stress that is specific to Nigeria's power sector: units that trip off and resynchronise frequently, or that see repeated load swings during grid disturbances, accumulate more thermal and mechanical cycling than a unit running steady baseload. Cyclic duty shortens hot section life relative to the fired-hours count alone, which is why a maintenance programme built purely on running hours can understate wear on a unit that starts and stops often.

## Maintenance philosophy: what actually protects the machine

Gas turbine maintenance is built around fired hours, equivalent operating hours (which weight starts and trips more heavily than steady running) and periodic inspection tiers rather than simple calendar intervals, because thermal cycling and fuel quality affect wear as much as raw running time.

The inspection hierarchy that most OEMs use, in increasing depth, typically runs: combustion inspection (combustor hardware and the first stage of the hot gas path, accessed through inspection ports), hot gas path inspection (turbine blading and vanes, usually needing partial disassembly), and major inspection or overhaul (full disassembly including the compressor and bearings). Borescope inspection through dedicated access ports lets an engineer look for coating loss, cracking and foreign object damage between scheduled outages without opening the casing.

Lube oil analysis, vibration monitoring and exhaust gas temperature spread across the turbine sections are the three condition indicators that most reliably give early warning of a developing problem, well before it shows up as a trip. See /blog/turbine-inspection-intervals/ for how inspection tiers are typically spaced against fired hours and starts.

Any work that involves opening casing access panels, isolating fuel gas supply, working near rotating shafts or entering the electrical isolation points on generator and excitation systems needs qualified personnel operating under a documented permit to work, with lockout and tagout applied to every energy source before anyone works on the machine. This is not a step-by-step guide to that isolation work, and it should not be treated as one.

Getting the inspection scope and findings documented properly, rather than guessed at from symptoms alone, is the difference between a planned outage that fixes the actual problem and a repeat trip a few months later. If your unit is showing wear patterns you cannot fully explain from the operating log, a power plant audit can establish the actual condition before you commit to an overhaul scope. For overhaul planning once a hot gas path or major inspection is confirmed, see /steam-turbine-overhaul-nigeria/, or request a technical proposal at /#contact.

## Reading the machine, not just the manual

A gas turbine that trips repeatedly, derates in harmattan season, or shows a widening exhaust temperature spread is telling you something specific about compressor fouling, fuel gas condition or hot section wear, not just that it needs "servicing." Understanding the Brayton cycle and where each symptom sits in the compression, combustion and expansion sequence is what turns a vague complaint into a scoped inspection.

For plants weighing a gas turbine against a diesel or gas reciprocating alternative, or trying to work out where a specific unit's degradation sits against a fleet-wide picture, a structured plant assessment gives a clearer basis for the next capital or maintenance decision than another round of guesswork on a running machine. Book a plant assessment through /#contact.

## Frequently Asked Questions

### How does a gas turbine actually generate power?

It compresses air, burns fuel with that compressed air to raise its temperature and pressure, then expands the hot gas through a turbine section. Part of the expansion work drives the compressor, and the remainder turns the output shaft connected to a generator or a mechanical drive load.

### What are the main parts of an industrial gas turbine?

The core sections are the air inlet and compressor, the combustor, and the turbine section, supported by auxiliary systems including lube oil, cooling and sealing air, fuel gas conditioning, instrumentation and the starting system. Each section can fail or degrade independently of the others.

### What is the difference between heavy-duty and aeroderivative gas turbines?

Heavy-duty frames are built for continuous baseload duty with slower starts and generally more tolerance for fuel variation. Aeroderivative units, adapted from aircraft engine cores, start faster and reach higher simple-cycle efficiency, which suits peaking and standby duty and mechanical drive applications where quick response matters.

### Why do gas turbines lose output during harmattan season in Nigeria?

Dust loading on the compressor inlet filters and fouling on compressor blading reduce compressor efficiency, which pushes firing temperature up for the same power output and can force a derate to protect hot section components. Filtration condition and cleaning schedule are the main levers available to limit this.

### How often should a gas turbine be inspected?

Inspection intervals are normally set against fired hours and equivalent operating hours, which weight starts and trips more heavily than steady running, rather than against a fixed calendar period. The OEM manual for the specific frame sets the actual combustion, hot gas path and major inspection intervals, and cyclic duty on the grid can bring those intervals forward.
