---
meta_title: "How a Thermal Power Plant Works: Cycle, Efficiency"
meta_description: "How a thermal power plant turns fuel into electricity, why combined cycle beats simple cycle on efficiency, and what drives upkeep on Nigerian sites."
primary_keyword: "thermal power plant"
secondary_keywords: "thermal power station, how a thermal power plant works, gas fired power plant, thermal plant efficiency"
---

# How a Thermal Power Plant Works: Cycle, Efficiency and Upkeep

If you manage a captive gas turbine set, sit on the O&M side of a gas-fired IPP, or specify a steam turbine for a process plant, you eventually need to defend a decision to your finance team or an auditor using the language of the cycle itself, not just "the generator is running fine." A thermal power plant is any generating unit that converts heat released from burning a fuel into mechanical shaft power, then into electricity. In Nigeria that fuel is overwhelmingly natural gas or associated gas, occasionally diesel or heavy fuel oil, and in a handful of process plants, biomass residues such as bagasse.

This article walks through the cycle itself, the two configurations you will meet on Nigerian sites, how efficiency is actually measured, and where the maintenance budget tends to go once the plant is running. It is written for people who have to plan, audit or defend that budget, not for a physics class.

## What a Thermal Power Plant Actually Does

Strip away the size and the site-specific equipment and every thermal power plant does the same three things: it burns fuel to release heat, it uses that heat to spin a turbine, and the turbine drives an alternator that produces electricity. The turbine can be a gas turbine, a steam turbine, or both in sequence. What differs between a small captive genset room and a large gas-fired IPP is scale, the number of stages the heat passes through before it is thrown away, and how tightly the plant is instrumented.

Two thermodynamic cycles cover almost everything you will find in Nigeria:

- The Brayton cycle, used by gas turbines: air is compressed, fuel is burned in that compressed air, and the hot expanding gas drives a turbine directly. No water is involved in the power cycle itself.
- The Rankine cycle, used by steam turbines: fuel heats water in a boiler or heat recovery steam generator (HRSG) to raise high-pressure steam, the steam expands through a turbine, and it is condensed and pumped back to the boiler to repeat.

A pure gas turbine plant runs the Brayton cycle only. A pure steam plant, such as a boiler feeding a back-pressure or condensing turbine at a process site, runs the Rankine cycle only. Where the two are joined, the exhaust heat a gas turbine would otherwise vent to atmosphere is instead routed through an HRSG to raise steam for a second turbine, which is what a combined cycle plant does.

## Simple Cycle Versus Combined Cycle

This distinction matters more to your fuel bill than almost any other design choice, and it has its own dedicated article if you want the fuller comparison: see [simple cycle vs combined cycle](/blog/simple-cycle-vs-combined-cycle/). The short version sits below.

In simple cycle, a gas turbine (or turbines) drives an alternator on its own and the hot exhaust, still well above 500 degrees Celsius, goes straight up the stack. Nothing recovers that heat. Simple cycle plants are cheaper to build, start faster, and tolerate frequent starts and stops far better than combined cycle plants, which is why they are common for peaking duty, fast-start emergency capacity, and remote or gas-constrained sites.

In combined cycle, the gas turbine's exhaust is captured by an HRSG to raise steam, and that steam runs a separate steam turbine, adding output from the same fuel input with no extra combustion. The trade-off is a bigger footprint, a longer and more expensive build, and less tolerance for rapid cycling, since the boiler and steam turbine sections do not like thermal shock.

| Configuration | Typical efficiency range | Typical heat rate | Where it tends to run |
|---|---|---|---|
| Simple cycle (gas turbine only) | roughly 33 to 43 percent | around 9,800 Btu/kWh (US EIA, 2015 generation data, published 2017) | Peaking, fast-start backup, remote or gas-constrained sites |
| Combined cycle (gas turbine plus HRSG plus steam turbine) | roughly 50 to 60 percent at design conditions | around 7,300 Btu/kWh (same EIA dataset) | Baseload IPPs and large industrial captive plants running long hours |

Those efficiency and heat rate figures are typical industry averages from the US Energy Information Administration's most recently published comparison of the two configurations, not a promise for any specific machine. The OEM's own performance curves for the exact turbine model, ambient conditions and fuel gas composition on your site govern what that unit will actually deliver, and derating for heat, humidity and dust changes the number further. Our [gas turbine explainer](/blog/gas-turbine-how-it-works/) covers what happens inside the Brayton side of either configuration in more depth.

## Heat Rate and Thermal Plant Efficiency

Heat rate is the working number a plant engineer actually uses day to day, and it is worth understanding before efficiency, not after. Heat rate is the amount of fuel energy, in Btu or kJ, needed to produce one unit of electrical output, typically expressed in Btu per kWh. A lower heat rate means less fuel burned for the same output, so heat rate and efficiency move in opposite directions: as heat rate falls, thermal efficiency rises.

The relationship in imperial units is straightforward:

Thermal efficiency (percent) is approximately equal to 3,412 divided by heat rate in Btu/kWh, then multiplied by 100.

Put a heat rate of 9,800 Btu/kWh into that formula and you get roughly 35 percent, in line with the simple-cycle range above. Put in 7,300 Btu/kWh and you get roughly 47 percent, again consistent with the combined-cycle figures. Two things push a real machine's heat rate away from its design number over its life: fouling of the compressor and hot gas path on the gas turbine side, and scaling or tube fouling on the steam side. Both are the reason inspection intervals exist rather than a nicety.

Take a hypothetical example to see why this matters commercially. A 30 MW simple-cycle gas turbine running continuously at a heat rate of 10,500 Btu/kWh instead of a clean 9,500 Btu/kWh is burning roughly 10 percent more fuel for the same electrical output, month after month, purely because of compressor fouling or a degraded combustion system. That gap does not show up as a single dramatic fault. It shows up as a fuel bill that creeps upward while the plant otherwise looks fine on the control room screen, which is exactly why heat rate needs to be tracked as a trend, not checked once a year.

## Where Thermal Plants Sit in Nigeria's Power Mix

Nigeria's grid runs almost entirely on thermal generation, with gas-fired plants making up the bulk of it and hydro filling most of the rest. Businessday NG reported in March 2026 that Nigeria's grid-connected installed generation base stood at 13,625 MW, citing individual thermal stations such as Egbin (1,320 MW) and Delta (900 MW) among the largest contributors. Availability on any given day tends to run well below that installed figure, for reasons that have more to do with gas supply, transmission constraints and plant condition than with turbine design, which is a separate discussion from the one in this article.

Outside the national grid, the same two cycles show up at smaller scale across the country: captive gas turbine sets at refineries and gas plants in the Niger Delta, gas engines and turbines behind the fence at manufacturing sites in Lagos and Ogun, and steam turbines running off process boilers at sugar mills, palm oil plants and some hospitals and universities. The physics does not change with size. The maintenance burden, discussed next, scales with it.

## What Actually Drives Maintenance on a Thermal Plant

A handful of factors account for most of the maintenance spend and most of the unplanned downtime on a thermal plant, whichever cycle it runs:

- Fuel and gas quality: contaminants, liquids in fuel gas, or off-spec diesel accelerate combustor and injector wear and can trigger trips.
- Inlet air quality: dust ingestion, harmattan conditions in particular, fouls the compressor and derates output. Our [harmattan dust derating article](/blog/harmattan-dust-turbine-derating/) covers this specifically.
- Hot gas path condition: combustor liners, transition pieces and turbine blades take the thermal and erosive load and are inspected on a schedule, not just when something fails. See [turbine inspection intervals](/blog/turbine-inspection-intervals/).
- Lubrication and bearing health: lube oil condition is a leading indicator on both gas and steam turbines, covered in [turbine lube oil analysis](/blog/turbine-lube-oil-analysis/).
- Steam and water chemistry, on any Rankine-cycle plant: scaling and corrosion in the boiler or HRSG and on turbine blading follow directly from poor feedwater treatment.
- Vibration and alignment across the rotating train: shaft misalignment, coupling wear and bearing degradation show up as vibration trends long before a forced outage.
- Controls and protection calibration: trip setpoints, sensing elements and governor tuning drift over time and need periodic verification. See [gas turbine trip causes](/blog/gas-turbine-trip-causes/).

Any work that involves isolating fuel gas or steam lines, opening a pressurised casing, or de-energising and re-energising alternator or switchgear circuits needs to be carried out by qualified personnel under lockout/tagout and a documented permit to work. That applies whether the unit is a 500 kVA diesel set or a large steam turbine train, and it is not a step to skip to save an outage window.

## Building an Inspection and Maintenance Programme Around the Cycle

A maintenance programme that actually protects heat rate and availability has to be built around the specific cycle running on site, not a generic checklist. A simple-cycle gas turbine plant needs an inspection regime keyed to combustion, hot gas path and compressor condition, following OEM-defined intervals in operating hours or starts, whichever governs first. A combined-cycle or standalone steam plant adds boiler or HRSG tube inspection, water chemistry monitoring and steam turbine internals to that list. Either way, a documented condition baseline, from a plant audit or diagnostic survey, gives you something to measure degradation against instead of guessing from the fuel bill months after the fact.

If your plant has never had a structured condition survey, or the last one predates the current operating regime, a [power plant audit and diagnostic assessment](/power-plant-audit-nigeria/) is the starting point before committing to an overhaul scope. For teams weighing a full turbine overhaul against continuing to patch, [steam and gas turbine overhaul services](/steam-turbine-overhaul-nigeria/) and a scoped technical proposal through [our contact page](/#contact) give you a fact-based comparison rather than a guess dressed up as a decision.

## Frequently Asked Questions

### What fuel do thermal power plants in Nigeria mostly use?

Natural gas and associated gas fuel most thermal generation on Nigeria's grid and behind the fence at industrial sites, with diesel and heavy fuel oil used where gas supply is unreliable or unavailable. A small number of process plants, such as sugar and palm oil mills, run steam turbines from boilers fired on biomass residue instead of fossil fuel.

### Is a thermal power plant the same thing as a power station?

A power station is the broader term for any facility that generates electricity for a grid or a site, and a thermal power plant is one category of power station, distinguished from hydro, solar or wind stations by the fact that it converts heat from burning fuel into mechanical and then electrical energy.

### Why does combined cycle reach higher efficiency than simple cycle?

Combined cycle captures the exhaust heat a simple-cycle gas turbine would otherwise vent to atmosphere and uses it to raise steam for a second turbine, extracting extra electrical output from the same fuel input rather than burning additional fuel to get it.

### What causes a thermal plant's heat rate to get worse over time?

Compressor fouling, hot gas path erosion or coating loss, and combustion system wear degrade a gas turbine's heat rate, while scaling, tube fouling and internal deposits do the same on the steam side of a Rankine-cycle plant. Both are the reason condition monitoring and scheduled inspection exist rather than running to failure.

### How is thermal plant efficiency actually calculated?

Efficiency is derived from heat rate: divide roughly 3,412 by the plant's heat rate in Btu per kWh and multiply by 100 to get an approximate efficiency percentage. The lower the heat rate, meaning less fuel burned per unit of electricity produced, the higher the resulting efficiency figure.
