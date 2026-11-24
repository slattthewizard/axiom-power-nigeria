---
title: "Generator Fuel Consumption per Hour: A Litres-per-Hour Chart by kVA and Load"
navTitle: "Generator Fuel Consumption per"
metaTitle: "Generator Fuel Consumption per Hour: Chart by kVA"
metaDescription: "Approximate generator fuel consumption per hour for 20 to 1000 kVA diesel sets at 25, 50, 75 and 100 percent load, with the formula and how to measure your own."
primaryKeyword: "generator fuel consumption per hour"
secondaryKeywords: "generator fuel consumption chart, diesel generator fuel consumption, litres per hour by kva, generator fuel consumption calculator"
publishedDate: "2026-11-24"
tag: "Generators"
subtitle: "Someone always asks the same question in a plant meeting: how much diesel does that set burn in an hour? The nameplate won't tell you."
canonical: "https://axiompowerng.com/blog/generator-fuel-consumption-chart/"
faq:
  - question: "How much diesel does a 500 kVA generator use per hour?"
    answer: "At a power factor of 0.8, a healthy 500 kVA set burns roughly 38 litres an hour at 25 percent load, about 60 at half load, about 84 at 75 percent and about 112 at full load. These are approximate working figures. Your own set could sit a few percent either side depending on make, age and condition."
  - question: "Does a generator use less fuel at half load?"
    answer: "It uses less fuel per hour, because it's producing less power, but it uses more fuel per kWh. At half load a typical diesel set burns around 0.30 litres per kWh, against about 0.28 at 75 percent and above. Below roughly 30 percent load the penalty gets larger, and the engine starts to suffer from wet stacking."
  - question: "Why is my generator using more fuel than the chart says?"
    answer: "First check the load. Many sets run far lighter than operators think, which pushes litres per kWh up. If the load is sensible, suspect injectors, a blocked air filter, a weak turbocharger or contaminated fuel. A measured test over a full shift, compared with the kWh meter, tells you which side of the line you're on."
  - question: "Can I use this chart for a gas or petrol generator?"
    answer: "No. The litres per kWh values here are for diesel engines. Gas and petrol engines have different efficiencies and different fuel units, so use data for that fuel and engine type instead."
---
Someone always asks the same question in a plant meeting: how much diesel does that set burn in an hour? The nameplate won't tell you. The OEM data sheet will, but only for the engine as shipped, new, on good fuel, at the load points the manufacturer chose to publish. What you actually burn depends on how hard the set is worked and what shape it's in.

This article gives you a working chart of approximate generator fuel consumption per hour for seven common sizes, the formula behind every number so you can rebuild the chart for your own set, and a way to measure the real figure on site. Treat every number here as an estimate. The measured figure on your own machine always wins.

## The formula behind the chart

Diesel generator fuel consumption per hour is the electrical power the set is delivering, multiplied by how many litres the engine needs to make each kilowatt-hour. That's it. The only trap is that sets are rated in kVA and fuel is burned per kW.

Litres per hour = kVA x 0.8 x load fraction x litres per kWh

The 0.8 is the power factor, which converts kVA to kW. If your load runs at a different power factor, the number changes, and our guide to [kVA to kW conversion](/blog/kva-to-kw-conversion/) walks through how to adjust. The load fraction is the share of the set's rated output you're actually drawing: 0.25, 0.5, 0.75 or 1.0.

The litres per kWh figure is the part that moves with load. The engine isn't equally efficient everywhere. For a healthy diesel set, typical values are:

- about 0.38 litres per kWh at light load, around 25 percent
- about 0.30 litres per kWh at half load
- about 0.28 litres per kWh at 75 percent and at full load

Those are textbook-style working values for a set in good condition, not a guarantee for any particular engine. Some makes do a bit better, tired ones do worse.

## Generator fuel consumption chart: litres per hour by kVA

Here's the chart. Each cell is kVA x 0.8 x load fraction x the litres per kWh figure for that load, rounded to the nearest 0.1 litre. All figures are approximate, assume a power factor of 0.8 and a healthy, well-maintained engine on clean fuel.

| Set size (kVA) | Rated kW at 0.8 | 25% load (0.38 L/kWh) | 50% load (0.30 L/kWh) | 75% load (0.28 L/kWh) | 100% load (0.28 L/kWh) |
|---|---|---|---|---|---|
| 20 | 16 | about 1.5 L/h | about 2.4 L/h | about 3.4 L/h | about 4.5 L/h |
| 60 | 48 | about 4.6 L/h | about 7.2 L/h | about 10.1 L/h | about 13.4 L/h |
| 100 | 80 | about 7.6 L/h | about 12.0 L/h | about 16.8 L/h | about 22.4 L/h |
| 200 | 160 | about 15.2 L/h | about 24.0 L/h | about 33.6 L/h | about 44.8 L/h |
| 300 | 240 | about 22.8 L/h | about 36.0 L/h | about 50.4 L/h | about 67.2 L/h |
| 500 | 400 | about 38.0 L/h | about 60.0 L/h | about 84.0 L/h | about 112.0 L/h |
| 1000 | 800 | about 76.0 L/h | about 120.0 L/h | about 168.0 L/h | about 224.0 L/h |

Take one row to see how it's built. A 200 kVA set at 75 percent load: 200 x 0.8 = 160 kW rated, 75 percent of that is 120 kW, and 120 kW x 0.28 L/kWh = 33.6 litres an hour. A 1000 kVA set at 25 percent: 1000 x 0.8 x 0.25 = 200 kW, and 200 x 0.38 = 76 litres an hour.

Notice what the chart does and doesn't show. Moving from half load to full load roughly doubles the hourly burn, which is just you making twice the power. What changes much less is the cost of each kilowatt-hour. That's the next section.

## Why light loading wastes fuel

Look at the litres per kWh column rather than litres per hour. At 25 percent load the engine burns about 0.38 litres for every kWh. At 75 percent it's about 0.28. A diesel engine has a fixed overhead: it has to turn itself, run its pumps and fans, and overcome friction whether or not the alternator is asking for much. Spread that overhead over a small output and every unit of electricity carries more fuel.

Take a hypothetical 500 kVA set. Suppose the plant needs 800 kWh over a shift. If the set runs at 25 percent load (100 kW), that's eight hours at about 38 litres an hour, roughly 304 litres. If the same energy were delivered at 75 percent load on a better-sized set, using 0.28 L/kWh, it's about 224 litres. That's around 80 litres of difference for the same electricity, every shift, with nothing wrong with the engine.

This is also where the hidden damage starts. Run a diesel lightly for long periods and combustion temperatures stay low. Unburnt fuel and soot build up in the exhaust, glaze the cylinder walls and foul the injectors. We cover that in detail in our piece on [diesel generator wet stacking](/blog/diesel-generator-wet-stacking/). The practical rule is simple. If a set lives below about 30 percent load, you don't have a fuel-saving problem, you have a sizing problem. Either run a smaller set for the base load, or consolidate loads so the set works at a sensible point.

Don't swing the other way and run it flat out, either. Continuous operation at the very top of the rating gives you no margin for a motor start or a harmonic-rich load, and it shortens the life of everything. A good working band for most prime-duty sets is somewhere around 60 to 80 percent of rated kW.

## How to measure your own set

The chart is a starting point. Your set has its own number, and you can measure it without special equipment. You need a fuel quantity, a time, and a kWh reading.

Method one is dipping the day tank. Fill the day tank to a marked level, run the set through a full shift on a normal load pattern, then top it up to the same mark using a calibrated container or a metered supply. The litres you add back is the fuel burned. A flow meter in the supply and return lines does the same job more neatly, and it's worth fitting if you do this regularly. Remember to subtract the return flow if the engine returns hot fuel to the tank, because only the net quantity counts.

Method two is pairing that fuel figure with kWh. Read the energy meter on the generator output at the start and end of the run. Then:

Litres per kWh = litres burned / kWh generated

Litres per hour = litres burned / hours run

Compare your litres per kWh against the working values above. If you're at 0.30 to 0.32 across a mixed shift with a modest load, you're about where you should be. If you're at 0.40 or higher and the set isn't lightly loaded, something is wrong.

A few notes so the test is honest:

- Use a full shift, or longer. Short tests exaggerate the effect of start-up and idling.
- Record the load, ideally from the controller's kW readout, at regular intervals. A mean of the readings is better than guessing.
- Check for leaks and weeping connections beforehand. A leak is fuel you paid for that never reached a cylinder.

If you're dipping a tank or working near the fuel lines, treat it as live equipment work. Isolate the set, apply lockout-tagout, and work under a permit to work. Don't open fuel lines on a running or startable machine, and keep ignition sources away from the area.

## What pushes consumption up

If the measured figure is well above the chart, the cause is nearly always one of a short list. Honestly, most of them are fuel system and air supply problems.

Worn or leaking injectors. A nozzle that dribbles or sprays a poor pattern burns fuel badly, makes smoke and raises litres per kWh while delivering less power. Pump timing drift does the same. If you see black smoke or rough running, our guide to [injector pump problems](/blog/injector-pump-problems/) is a good place to start.

Blocked air filters. The engine needs a fixed ratio of air to fuel. Restrict the air and combustion goes rich, fuel use rises and smoke follows. In dusty seasons this can happen faster than the service interval assumes, so look at the restriction indicator rather than the calendar.

A tired turbocharger. If the turbo isn't delivering its boost pressure, the engine is short of air and compensates by burning poorly. Oil leaks at the turbo seals, a whine, or low boost on the gauge all point this way.

Overload. Pushing the set beyond its rating makes it burn more per kWh, runs temperatures up and eventually trips the set or damages it. It's the quickest way to turn a fuel problem into a repair bill.

## Using the numbers in planning

Once you have a chart that matches your own measured data, it becomes a planning tool. For a given daily run pattern you can multiply the litres per hour by hours at each load level to forecast daily and monthly litres, and compare that against the stock you keep on site. The same arithmetic feeds the cost side of the business. Our guide to [diesel generator cost per kWh](/blog/diesel-generator-cost-per-kwh/) shows how the litres per kWh figure combines with fuel cost and maintenance to give a true per-unit cost, which is what you compare against any grid or alternative supply.

If you're sizing a new set, the chart is a reminder to size for the load you really have, not the load you might one day have. An oversized set sitting at 20 percent costs more per kWh every hour it runs. Where the load varies widely, two smaller sets that share duty often beat one large one.

## Get your own numbers checked

If your measured fuel use sits well above these figures, or you'd like a sizing and loading review before buying more capacity, [request a technical proposal](/#contact) and our engineers will take a look on site.

## Frequently Asked Questions

### How much diesel does a 500 kVA generator use per hour?

At a power factor of 0.8, a healthy 500 kVA set burns roughly 38 litres an hour at 25 percent load, about 60 at half load, about 84 at 75 percent and about 112 at full load. These are approximate working figures. Your own set could sit a few percent either side depending on make, age and condition.

### Does a generator use less fuel at half load?

It uses less fuel per hour, because it's producing less power, but it uses more fuel per kWh. At half load a typical diesel set burns around 0.30 litres per kWh, against about 0.28 at 75 percent and above. Below roughly 30 percent load the penalty gets larger, and the engine starts to suffer from wet stacking.

### Why is my generator using more fuel than the chart says?

First check the load. Many sets run far lighter than operators think, which pushes litres per kWh up. If the load is sensible, suspect injectors, a blocked air filter, a weak turbocharger or contaminated fuel. A measured test over a full shift, compared with the kWh meter, tells you which side of the line you're on.

### Can I use this chart for a gas or petrol generator?

No. The litres per kWh values here are for diesel engines. Gas and petrol engines have different efficiencies and different fuel units, so use data for that fuel and engine type instead.
