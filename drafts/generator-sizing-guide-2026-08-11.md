---
meta_title: "How to Size a Generator for a Factory: kVA, Step Loads"
meta_description: "How to size a generator for a factory in Nigeria: measured load profiles, kVA maths, motor step loads, harmonic derating and realistic NGN cost figures."
primary_keyword: "how to size a generator for a factory"
secondary_keywords: "generator sizing for a factory, standby generator kVA calculation, factory generator size Nigeria, motor step load generator sizing, harmonic derating generator"
---

# How to Size a Generator for a Factory: kVA, Step Loads and Harmonic Loads

A plastics plant in a Lagos industrial estate commissioned a 500 kVA standby set, ran it for eleven months, and then lost a full production shift when the alternator regulator failed under harmonic stress. The set was never undersized on running load. It was sized on the sum of motor nameplates and nothing else, which is how most factories in Nigeria end up with a machine that is simultaneously too big for its fuel bill and too weak for its worst moment. Learning how to size a generator for a factory properly means separating three different questions: what the plant draws continuously, what it demands in the half second a large motor starts, and what shape the current waveform is in when it gets there.

Getting this wrong is expensive in both directions. Undersize and you buy voltage dips, nuisance trips and early alternator failure. Oversize and you pay for capex you never use, then run at a load factor low enough to cause wet stacking.

## Why Nameplate Addition Is the Most Expensive Mistake in Generator Sizing

The default method on most Nigerian sites is to walk the plant, add up every motor and heater nameplate, divide by 0.8, then add a comfort margin. This produces a number that is almost always 60 to 100 per cent above what the factory actually needs.

The reason is diversity. No industrial plant runs every load at full rating at the same instant. Conveyors idle, compressors unload, extruders sit at soak drawing a fraction of heater nameplate, and standby pumps do what their name says.

Consider a feed and flour mill on a northern industrial estate. Connected nameplate across hammer mills, the pellet press, roller stands, conveyors and dust extraction came to 1,180 kW. Two weeks of logging at the main incomer showed maximum demand of 512 kW and an average of 361 kW. The nameplate method pointed at a 1,500 kVA set at roughly NGN 186 million (about USD 120,000 at prevailing rates). The measured method, with proper step load headroom added, landed on 800 kVA at roughly NGN 108 million (about USD 70,000).

That is NGN 78 million of avoided capex, before counting the fuel penalty of running a 1,500 kVA machine at a 24 per cent load factor for its whole life. If you are at the specification stage and working from nameplate totals, [request a technical proposal](/#contact) before the purchase order goes out. A load study costs a fraction of the sizing error it prevents.

## How to Size a Generator for a Factory: Start With a Measured Load Profile

The load study is not a walk-around. It means a power quality logger clamped at the main incomer and at any sub-board feeding a large or non-linear group, left in place for seven days minimum and preferably fourteen, sampling fast enough to capture starting events.

What you are collecting is five things:

- Maximum demand in kW and kVA, with the timestamp so you can tie it to a production event
- Average demand and load factor across the logging window
- Displacement power factor and true power factor at the incomer
- Total harmonic distortion of current, THD(i), and the individual harmonic orders
- The magnitude and duration of every step load event, especially direct-on-line motor starts

Fourteen days matters because most factories have a weekly rhythm. A mill that runs one shift Monday to Wednesday and two shifts Thursday to Saturday has a very different peak profile from what a Tuesday afternoon site visit would suggest.

If the plant is not yet built you must construct the profile from process data: machine duty cycles, expected simultaneity and the commissioning sequence. Say so in the specification, size conservatively on step load, and re-verify with a logger after three months of production. Anyone giving a firm kVA number for an unbuilt plant without asking for a duty cycle table is guessing.

## kVA, kW and Power Factor: Getting the Arithmetic Right

A generator set carries two independent ratings and both can be the binding constraint. The engine is rated in kW and limits real power. The alternator is rated in kVA and limits apparent power, because it is the current that heats the windings.

Standard sets are rated at 0.8 power factor lagging, so a 500 kVA set is a 400 kW set. If your measured demand is 400 kW at a true power factor of 0.72, you are asking for 556 kVA and the alternator is overloaded even though the engine is not.

This is where power factor correction earns its place. Correcting a plant from 0.72 to 0.95 on the same 400 kW demand drops the apparent power requirement from 556 kVA to 421 kVA. That is often the difference between an 800 kVA set and a 500 kVA set, and capacitor banks are far cheaper than alternator frames.

Two cautions apply. Capacitors sized for utility supply overcorrect on generator, and a leading power factor into an alternator causes voltage regulation instability. You need detuned reactors and a controller with a generator mode, not a fixed bank, because undetuned capacitors on a plant with heavy drive content will resonate with the harmonic spectrum and fail.

Use ISO 8528-1 rating definitions rather than vendor marketing labels. Prime power, limited time running power and standby power are different duty classes with different permitted load factors, and the definitions are set out in [ISO 8528-1](https://www.iso.org/standard/68539.html). A set quoted at 500 kVA standby is not a 500 kVA prime mover.

## Step Loads Usually Decide the Set Size, Not Running Load

The single largest motor started direct-on-line will draw six to eight times full load current for one to three seconds, at a power factor of about 0.2. The alternator has to supply that current while holding voltage inside the tolerance your controls will accept, and the engine has to absorb the torque step without frequency dipping below the underfrequency trip.

Transient voltage dip is governed largely by the alternator subtransient reactance, X"d. A standard machine sits around 14 to 18 per cent. A machine specified at 10 to 12 per cent will hold voltage far better on the same kVA, and specifying reactance is usually cheaper than specifying a bigger set.

A cold store and fish processing facility in Rivers State ran into this on commissioning. A 160 kW screw compressor started direct-on-line, inrush measured at 6.5 times full load current, and the 500 kVA set dipped 24 per cent at the busbar. The PLC dropped out at its 18 per cent undervoltage threshold, taking the whole refrigeration pack down with it.

Two options were costed. Upsizing to an 800 kVA set added roughly NGN 46 million. Fitting a soft starter on the compressor and re-verifying the dip cost NGN 4.2 million (about USD 2,700) and brought the dip to 11 per cent. The soft starter won on every measure.

Decide your starting method before you order the set. Star-delta roughly halves inrush but produces an open transition spike unless it is a closed transition unit. Soft starters give a controlled ramp and pass harmonics while ramping. Drives remove the transient altogether and add a permanent harmonic load instead. Sequencing large motors so they never start together costs nothing and is routinely overlooked, so [book a plant assessment](/#contact) and get the sequence written into the control philosophy rather than discovered at commissioning.

## Harmonic Loads: VFDs, Rectifiers and Alternator Uprating

A generator is a much weaker harmonic source than the utility. Its source impedance is an order of magnitude higher, so the same non-linear load that produces 6 per cent voltage distortion on grid supply can produce 15 to 20 per cent on generator.

Six-pulse VFDs, UPS rectifiers, LED driver banks, induction heaters and switch-mode supplies all draw current in pulses rather than sinusoids. The dominant orders are the 5th, 7th, 11th and 13th. Those currents circulate in the alternator windings, produce no useful torque, and heat the machine.

The practical rules that hold on most Nigerian industrial sites:

- Below about 20 per cent non-linear load as a share of total, a standard alternator with a 2/3 pitch winding is generally adequate
- Between 20 and 40 per cent, uprate the alternator one frame size while keeping the engine, and specify a permanent magnet or auxiliary winding excitation system so the AVR does not lose reference on a distorted waveform
- Above 40 per cent, a harmonic study is needed and passive or active filtering should be costed alongside the set

The Lagos plastics plant mentioned at the top is the case in point. Twenty-two injection moulding machines, fourteen on six-pulse drives, measured THD(i) of 28 per cent at the main incomer with the plant on generator. The corrective specification was a 500 kVA engine with an uprated alternator at 625 kVA frame, 2/3 pitch winding, PMG excitation and a digital AVR with harmonic-tolerant sensing. The delta over a standard 500 kVA set was about NGN 14 million (roughly USD 9,000), against a lost shift that the plant costed at NGN 9.6 million.

Distortion limits and measurement methodology are covered in [IEEE 519](https://standards.ieee.org/ieee/519/10677/). If your plant already sees flicker, overheating neutrals or transformer noise, harmonic content is the first thing worth measuring, and it overlaps with the symptoms in [generator low output causes](/blog/generator-low-output-causes/).

## Site Derating, Oversizing and What It All Costs

Every set is rated at reference conditions, typically 25 degrees Celsius ambient, 100 metres altitude and 30 per cent relative humidity. Nigerian conditions are not those conditions.

Expect roughly 2 to 4 per cent output loss per 5 degrees above 25 degrees ambient, and 1 to 3 per cent per 300 metres above reference altitude. A canopied set in an unventilated Lagos plant room can sit 12 degrees above outside ambient, which quietly removes 6 to 9 per cent of its rating. Plant room ventilation is part of sizing, not an afterthought.

Harmattan dust is a real derating factor in the north. Restricted air filters raise intake depression and pull output down, and the effect compounds with high ambient. The same physics applies to turbomachinery, which we cover in [harmattan dust turbine derating](/blog/harmattan-dust-turbine-derating/).

Oversizing carries its own bill. A diesel set run below about 30 per cent load for extended periods does not reach cylinder temperatures high enough for complete combustion. The result is wet stacking: unburnt fuel and carbon in the exhaust, glazed bores, fouled turbochargers and injectors, and a set that needs unscheduled overhaul years early.

| Sizing basis | Set specified for the 512 kW mill | Indicative capex | Consequence |
|---|---|---|---|
| Sum of nameplate ratings, no diversity | 1,500 kVA | NGN 186m (USD 120,000) | 24% load factor, wet stacking, NGN 78m wasted capex |
| Utility maximum demand from bills | 630 kVA | NGN 78m (USD 50,000) | Adequate running load, fails on 132 kW motor start |
| Vendor rule of thumb, kW / 0.8 plus 25% | 1,180 kVA | NGN 158m (USD 102,000) | Same wet stacking exposure, no harmonic provision |
| 14-day logged profile plus step load study | 800 kVA | NGN 108m (USD 70,000) | 64% load factor, dip held under 12%, correct alternator spec |

Figures are indicative for August 2026 and vary with brand, canopy, controller, switchgear scope and exchange rate. Fuel is the larger number over a ten year life in any case, and we break that down in [diesel generator cost per kWh](/blog/diesel-generator-cost-per-kwh/).

One honest note on hybrids. Solar PV with battery storage genuinely reduces diesel hours and fuel spend on daytime base load, and on a single-shift factory it can be a strong investment. It does not change the kVA you need. PV inverters are current-limited devices and cannot deliver the six-times inrush a direct-on-line motor demands, so the generator still has to be sized for the worst step load even if it runs far fewer hours. Anyone telling you solar lets you buy a smaller set is describing a plant with no large motors.

The load profile keeps moving as production changes, so re-log every two or three years and fold the result into the [generator maintenance](/generator-maintenance-nigeria/) schedule. For plants with multiple sets, synchronising panels or a mix of generation and utility supply, a full [power plant audit](/power-plant-audit-nigeria/) is the better starting point. To scope either, [request a technical proposal](/#contact) or call +234 803 000 0000.

## Frequently Asked Questions

### How much bigger than my measured load should the generator be?

There is no single margin, because the binding constraint differs by plant. With modest motors and mostly resistive load, 15 to 20 per cent above measured maximum demand is usually enough. With a large direct-on-line motor, the step load calculation can demand 60 per cent or more headroom, and the right answer is often a soft starter plus a smaller set.

### Can I use my electricity bill to size the generator?

It is a sanity check on running load and nothing more. Utility maximum demand is integrated over 15 or 30 minutes, so it averages away the sub-second transients that decide whether your alternator holds voltage. Bills also say nothing about harmonic content or power factor at the moments that matter. Use them to validate a logged profile, not to replace one.

### Do variable frequency drives mean I can buy a smaller generator?

Partly, and with a trade-off. VFDs remove the motor starting transient, which usually lets you drop the step load allowance and specify a smaller engine. In exchange they add continuous harmonic current, so above roughly 20 per cent drive content you must uprate the alternator frame, specify PMG excitation and possibly add filtering. The net cost effect is usually favourable but it is not automatic.

### How long does a proper load study take and what does it involve?

Plan for a site visit to install loggers at the main incomer and relevant sub-boards, fourteen days of logging to capture the weekly rhythm, then analysis and a written sizing report. Installation needs either an isolation or a live-working procedure depending on the switchboard, so a qualified engineer must attend and production must agree a short access window. Where there is no safe clamping point, an outage window is required and we will say so before quoting.
