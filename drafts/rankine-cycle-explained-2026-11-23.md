---
meta_title: "Rankine Cycle Explained: Steam Plant Efficiency Guide"
meta_description: "The Rankine cycle in plain engineering terms: the four processes, ideal vs actual cycle, what lifts efficiency and what drags a steam plant below design."
primary_keyword: "rankine cycle"
secondary_keywords: "rankine cycle diagram explained, steam power plant cycle, rankine cycle efficiency, reheat and regenerative rankine cycle"
---

# Rankine Cycle Explained: How a Steam Plant Turns Heat into Power and Where It Loses It

Every steam turbine on a Nigerian site, whether it sits behind a gas-fired boiler, a biomass boiler or a waste heat recovery unit, runs on the same thermodynamic loop. That loop is the Rankine cycle. Textbooks draw it as a neat shape on a chart. On a plant it's a feed pump, a boiler, a turbine and a condenser, plus a few hundred valves and a lot of pipe, and the gap between the neat shape and your actual heat rate is where the money goes.

This article walks through the cycle the way a field engineer would. First the four processes, then what the T-s diagram is telling you, then the difference between the ideal cycle and the one you're running. After that, what raises efficiency by design, and what drags a real plant below its design figure. If you want the wider picture of how a whole station fits together, start with our guide to the [thermal power plant](/blog/thermal-power-plant-explained/) and come back here for the cycle itself.

## The four processes in the steam power plant cycle

Water goes round a closed loop. It changes phase twice, from liquid to steam in the boiler and back to liquid in the condenser, and that's the whole trick.

Feed pump (compression). Condensate at low pressure is pumped up to boiler pressure. Because it's liquid and nearly incompressible, this takes very little work compared with what the turbine gives back. That's the entire reason a steam cycle beats a gas cycle on back work: compressing a liquid is cheap, compressing a gas isn't. The pump is small, but if it's worn or the suction is poor, the whole plant feels it.

Boiler (heat addition). Heat from fuel goes into the water at roughly constant pressure. The water is first warmed to saturation in the economiser, boiled in the furnace walls and drum, then dried and heated further in the superheater. Fuel type doesn't change the cycle. It changes the boiler.

Turbine (expansion). High pressure, high temperature steam expands through the blading, drops in pressure and temperature, and turns the shaft. This is where the useful work comes out. For how the nozzles, blades and casing actually do that, see [how a steam turbine works](/blog/steam-turbine-how-it-works/).

Condenser (heat rejection). Exhaust steam is condensed on cooled tubes at a pressure well below atmosphere, typically somewhere in the region of 5 to 10 kPa absolute on a water-cooled unit. The condensate is collected in the hotwell and the extraction pump sends it back toward the feed pump. The heat that leaves here is the largest single loss in the cycle, and it's the one you can't escape. You can only reject it at the lowest temperature your cooling water allows.

## Reading the T-s diagram in words

You don't need the picture to follow it. Imagine temperature going up the vertical axis and entropy along the bottom, with a dome-shaped curve in the middle. Under the dome, steam and water coexist. To the left of it is liquid, to the right is dry vapour.

Start at the condenser outlet, a saturated liquid at low temperature, sitting at the left foot of the dome. The feed pump moves the state almost straight up, a tiny step because liquid compression barely changes anything. Then the boiler: the line climbs along the liquid side, runs flat across the dome while the water boils at constant temperature, and keeps rising into the superheated region on the right as the superheater adds heat. The area under that path is the heat put in.

The turbine is, ideally, a straight vertical drop at constant entropy, back down toward the dome and to a lower temperature. Then the condenser closes the loop by running flat along the bottom, with the steam condensing back to saturated liquid at constant pressure and temperature.

Two things to take from the shape. The enclosed area is the net work. And the efficiency is that area divided by the heat put in, so anything that makes the average temperature of heat addition higher, or the temperature of heat rejection lower, widens the shape and improves efficiency. Every improvement later in this article is one of those two moves.

## Ideal cycle versus the actual cycle

The ideal Rankine cycle assumes the pump and turbine are perfect (constant entropy) and that there's no pressure drop in the boiler, the pipework or the condenser. None of that is true.

In the real cycle the turbine isn't isentropic. Friction, leakage over the blade tips and wet steam at the exhaust mean the exit state is hotter and wetter than the ideal one, so you get less work per kilogram of steam. The ratio of actual to ideal enthalpy drop is the isentropic efficiency, and on a healthy large turbine it's typically somewhere in the high 80s percent, lower on small machines and lower still when the blading is dirty or damaged. The feed pump isn't perfect either, though it matters less. Then add pressure drop through the superheater, the main steam line and the stop and control valves, plus heat lost from every uninsulated flange.

Honestly, this is why a design heat rate on a datasheet and the figure you see on a Tuesday afternoon don't match. A subcritical plant of the kind common in industry typically sits in the region of 30 to 40 percent cycle efficiency by design. Small industrial back-pressure and condensing sets are usually below that. The datasheet number is the starting point, and every defect below subtracts from it.

## What raises Rankine cycle efficiency by design

These are choices made when a plant is specified, not things you adjust on a shift. It's worth knowing them because they explain why two machines of the same rating can have very different fuel consumption.

Higher steam pressure and temperature. Raising boiler pressure and superheat temperature lifts the average temperature at which heat enters, so the cycle widens at the top. The limit is metallurgy: creep strength of the tubes, headers and turbine casings sets how hot you can go. Higher pressure alone also leaves the exhaust wetter, which brings us to reheat.

Lower condenser back-pressure. This is the other end of the shape. A better vacuum lets the turbine expand the steam further and extract more work. The floor is set by cooling water temperature, because the condenser can't get colder than the water cooling it. In a Nigerian climate, with warm cooling water for much of the year, that floor is higher than in a temperate country, and that is a design reality, not a defect.

Reheat. After partial expansion in the high pressure turbine, the steam goes back to the boiler to be heated again, then continues through the intermediate and low pressure sections. That does two jobs. It raises the average heat addition temperature slightly, and more importantly it keeps the steam dry enough toward the exhaust, because moisture erodes the last stage blades. Reheat only pays on larger, higher pressure plants. On a small industrial set the extra boiler complexity isn't worth it.

Regenerative feedwater heating. Instead of sending all the steam to the condenser, a little is bled from the turbine at several points and used to warm the feedwater before it reaches the boiler. That steam gives up its heat to the feedwater instead of rejecting it to the cooling water, and the water enters the boiler hotter, so less fuel is needed to bring it to boiling. Large stations use several stages of heaters plus a deaerator, and between them they account for much of the difference between a basic cycle and a good one. The plain combined effect of reheat and regeneration is what people mean by a reheat and regenerative Rankine cycle, and it's what almost every large steam unit actually runs.

If your machine exhausts at a pressure above atmosphere to feed a process instead of a condenser, you're running a different arrangement with different trade-offs. We cover that in [back-pressure versus condensing turbines](/blog/back-pressure-vs-condensing-turbine/).

## What drags a real plant below design

Now the useful part. Most plants don't lose efficiency because of the design. They lose it to a short list of things that creep in over months. Here they are, with what to look at.

| Loss | What it does to the cycle | What to check |
|---|---|---|
| Condenser tube fouling | Raises tube wall resistance, so back-pressure climbs for the same load | Condenser pressure against cooling water inlet temperature, terminal temperature difference, tube cleanliness at shutdown |
| Air in-leakage | Air blankets the tubes and raises the exhaust pressure; the air ejectors or vacuum pumps work harder | Vacuum pump or ejector load, subcooling of condensate, a vacuum decay test with the unit isolated |
| Warm cooling water | Lifts the lowest temperature the condenser can reach | Cooling tower approach, fan and fill condition, basin level and temperature, river or sea inlet temperature |
| Steam leaks and passing valves | Steam that does no work, plus make-up water and fuel to replace it | Drain and vent valve tail pipes that stay hot, bypass valves, unexplained make-up water demand |
| Turbine deposits | Rough or deposited blades cut flow capacity and isentropic efficiency; stage pressures rise | Stage pressure trends against load, steam purity records, carryover from the boiler |
| Feedwater heaters out of service | Feedwater enters the boiler colder, so more fuel is burned for the same output | Terminal temperature differences, heater drain levels, extraction line valves, tube leaks |
| Gland seal and shaft leakage | Steam or air passing where it shouldn't, upsetting both output and vacuum | Gland steam pressure, gland condenser performance, leak-off flows |

A few of these deserve a comment, because that's where most of the trouble lives.

Condenser fouling and air in-leakage are the two that cost the most, and they look alike on the gauge: back-pressure goes up. The way to tell them apart is to compare condenser pressure with the saturation pressure for the temperature of the condensate. A large gap points to air. A normal gap with a high terminal temperature difference points to dirty tubes or poor cooling water flow. Chasing the wrong one wastes a shutdown.

Passing valves are the quiet thief. A steam trap or drain valve that doesn't fully seat can pass a meaningful amount of steam straight to the condenser or the atmosphere, and you pay for that steam twice, once in fuel and once in treated make-up water. A thermal image or a hand-held thermometer on the downstream side of each drain, taken at steady load, finds most of them. The usual tell is a downstream pipe that is as hot as the upstream one when the valve should be closed.

Turbine deposits are a boiler-side problem that shows up in the turbine. If the steam carries silica, salts or carryover from the drum, they plate out on the nozzles and blades. You'll see first-stage pressure creeping up at constant load, or output slipping with no change in steam flow. This one connects directly to feedwater and boiler chemistry, and it's why steam purity records matter as much as the turbine log.

A word on safety. Almost every check above can be done from the control room or with the unit running, but anything that means opening a condenser water box, working on a heater, or putting hands on a valve or drain needs the equipment isolated, locked out and tagged out, and a permit to work issued before anyone starts. Steam lines and heaters hold stored energy and heat long after they look quiet.

## A quick hypothetical to size the vacuum problem

Take a hypothetical condensing steam turbine running at a steady load with a design condenser pressure of 8 kPa absolute. Over a season the tubes foul and a gland seal starts to pull in air, and the back-pressure drifts to 12 kPa. The turbine now has less pressure ratio to expand across, so for the same steam flow it produces less power, and to hold output the boiler has to be fired harder. A 4 kPa drift sounds small on a gauge, but the exhaust conditions change enough that you'd expect a visible fall in output and a visible rise in fuel for the same load. That's the sort of drift a monthly trend would catch long before a shutdown inspection would.

The point isn't the specific numbers, which will differ on every machine. It's that vacuum is the cheapest efficiency you'll ever recover, and it's the one most plants stop watching once commissioning is over.

## Where the Rankine cycle sits in combined cycle plants

Rankine doesn't only live in steam-only stations. A combined cycle plant is a gas turbine on top and a steam turbine below. The gas turbine exhaust, still at several hundred degrees Celsius, passes through a heat recovery steam generator (HRSG), which is effectively a boiler with no furnace. The steam it raises runs a Rankine cycle: steam turbine, condenser, feed pump, and often multiple pressure levels with reheat to extract as much as possible from the exhaust heat. That bottoming cycle is why combined cycle plants reach efficiencies a simple-cycle gas turbine can't. If you're weighing the two arrangements, we compare them in [simple cycle versus combined cycle](/blog/simple-cycle-vs-combined-cycle/).

## Putting it to work on your plant

If you operate or maintain a steam turbine, there are three numbers to trend every week at similar load: condenser pressure against cooling water temperature, final feedwater temperature, and first-stage or governing stage pressure. Together they tell you about the condenser, the heaters and the blading, which covers most of what the table above describes. A flat line is good. A slow climb is a job waiting to be scheduled.

When the trends point at the machine itself, such as deposits, damaged blading or worn seals, the fix usually needs the casing open, and that's work for a planned outage with proper inspection. Our team covers that under [steam turbine overhaul in Nigeria](/steam-turbine-overhaul-nigeria/), and a plant audit can sort out whether the loss is in the cycle, the boiler or the auxiliaries before anyone commits to opening anything up.

If your steam plant is burning more fuel per megawatt-hour than it did a few years ago and you don't know why, [request a technical proposal](/#contact) and our engineers will help you find where the heat is going.

## Frequently Asked Questions

### What is the Rankine cycle in simple terms?

It's the closed loop that almost every steam power plant uses. Water is pumped to high pressure, boiled into steam in a boiler, expanded through a turbine to produce shaft power, then condensed back to water and returned to the pump. The turbine's work output minus the small pump work is what you get as electricity.

### How efficient is the Rankine cycle?

Typical ranges depend on the plant. A basic industrial steam cycle is often in the 20 to 30 percent range, large subcritical utility units are commonly 30 to 40 percent, and advanced supercritical units can be higher. Where your plant falls depends on steam conditions, condenser vacuum, reheat and feedwater heating, and how well it's maintained.

### Why does condenser vacuum matter so much?

The lower the exhaust pressure, the more energy the turbine can extract from each kilogram of steam, so output goes up for the same fuel. When fouling or air in-leakage worsens the vacuum, the turbine produces less and the boiler has to burn more to compensate. It's usually the first place to look when a unit underperforms.

### What's the difference between reheat and regenerative cycles?

Reheat takes partly expanded steam back to the boiler for a second heating before it finishes expanding, which raises output and keeps exhaust steam drier. Regenerative heating bleeds some steam from the turbine to pre-warm the feedwater, so the boiler has less heat to add. Most large plants use both together.

### Do combined cycle plants use the Rankine cycle?

Yes. The steam side of a combined cycle plant is a Rankine cycle. A heat recovery steam generator captures heat from the gas turbine exhaust and raises steam, which drives a steam turbine, condenser and feed pump just as in a conventional steam plant.
