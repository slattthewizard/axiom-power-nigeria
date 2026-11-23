---
meta_title: "Heat Rate in Power Plant: Formula and Calculation"
meta_description: "Heat rate in a power plant is the fuel energy burned per kWh sent out. See the formula, a worked example, LHV vs HHV and what makes heat rate drift."
primary_keyword: "heat rate in power plant"
secondary_keywords: "heat rate formula, heat rate calculation, heat rate vs efficiency, gas turbine heat rate"
---

# Heat Rate in a Power Plant: Formula, Calculation and What Makes It Drift

Ask a plant manager how the plant is doing and you'll usually hear about availability, trips and fuel supply. Ask how much fuel energy it takes to make one kWh and you'll often get a pause. That number is the heat rate, and it's the closest thing a thermal plant has to a fuel economy figure.

Fuel is the biggest running cost on almost every gas, diesel or steam plant, and heat rate is how you tell whether you're burning more of it than you should. A unit can be fully available and still be quietly wasting several percent of its fuel.

## What heat rate actually measures

Heat rate is the fuel energy you put in for each unit of electricity you get out. The usual units are kJ/kWh, or Btu/kWh in American-influenced documents and some OEM paperwork. Lower is better. A plant at 10,000 kJ/kWh does the same job as one at 12,000 kJ/kWh while burning a sixth less fuel.

It's a ratio of two measurements, fuel energy and electrical output, and either one can be wrong. It also covers the whole unit. On a steam plant the boiler, turbine, condenser and feed pumps all show up in the one number. When heat rate moves, something in the chain has changed, and the job is finding which link.

## The heat rate formula and a worked calculation

The formula is short:

Heat rate = fuel energy input (kJ) / electrical energy output (kWh)

Fuel energy input is the quantity of fuel burned multiplied by its calorific value. Output is the electricity measured at a defined point, which we'll get to shortly.

Here's a hypothetical gas turbine generator set running steady at full load. In one hour it produces 20,000 kWh at the generator terminals. The fuel gas meter and a gas analysis say the fuel burned in that hour carried 240,000 MJ of energy, on a lower heating value basis.

Convert to kJ first, because that's where people slip: 240,000 MJ is 240,000,000 kJ. Then divide.

Heat rate = 240,000,000 kJ / 20,000 kWh = 12,000 kJ/kWh

In Btu terms, divide by 1.055 and you get roughly 11,400 Btu/kWh.

Now suppose compressor fouling pushes that heat rate up by 3 percent, to 12,360 kJ/kWh. At the same 20,000 kW output, the unit burns 7,200 MJ more fuel every hour (3 percent of 240,000 MJ). No alarm, no trip. The fuel bill would notice.

## Heat rate vs efficiency

Heat rate and efficiency are the same information written two ways. One kWh is 3,600 kJ, so:

Efficiency = 3,600 / heat rate (in kJ/kWh)

For the example above, 3,600 / 12,000 = 0.30, so 30 percent. In Btu, use 3,412 in place of 3,600: 3,412 / 11,373 gives the same 30 percent.

Efficiency is easier to grasp on a slide. Heat rate is easier to work with, because a 1 percent change in heat rate is a 1 percent change in fuel at the same output. Going from 30 percent to 29.1 percent efficiency doesn't sound like much until you work out it's 3 percent more fuel.

## Gross vs net, LHV vs HHV

Gross heat rate divides the fuel energy by the output at the generator terminals. Net heat rate divides it by what's left after the plant's own auxiliaries, such as fuel gas compressors, cooling fans, lube oil pumps and boiler feed pumps. Say the hypothetical set's auxiliaries draw 500 kW. Net output is 19,500 kWh for that hour, so:

Net heat rate = 240,000,000 / 19,500 = about 12,308 kJ/kWh

Net efficiency is 3,600 / 12,308, about 29.25 percent. Same machine, same hour, a worse-looking number. Net is the honest one for cost, because you pay for the fuel that ran the auxiliaries too.

The second trap is the heating value. The higher heating value (HHV) counts the energy released when the water vapour from combustion condenses. The lower heating value (LHV) doesn't. For natural gas the HHV is roughly 10 percent above the LHV. Our unit's 240,000 MJ on an LHV basis becomes about 264,000 MJ on an HHV basis. The gross heat rate is then 264,000,000 / 20,000 = 13,200 kJ/kWh, and the efficiency falls to about 27.3 percent.

Nothing changed in the plant, only the accounting. OEM datasheets are usually on LHV, while some utility reporting uses HHV. Before comparing your plant to a datasheet or a contractor's claim, find out which basis, and gross or net, each figure uses. Half the disputes on this subject end there.

## Typical heat rate by plant type

Textbook ranges for healthy machines, on an LHV basis and roughly gross. Real plants sit inside them or just outside.

| Plant type | Heat rate (kJ/kWh) | Efficiency |
|---|---|---|
| Small industrial gas turbine, simple cycle | 10,000 to 14,000 | 26 to 36 percent |
| Gas turbine combined cycle | 6,200 to 7,500 | 48 to 58 percent |
| Subcritical steam plant | 9,500 to 11,000 | 33 to 38 percent |
| Gas engine generator | 8,500 to 10,000 | 36 to 42 percent |
| Diesel generator at 75 to 100 percent load | 9,700 to 10,800 | 33 to 37 percent |

The diesel row matches the fuel figures most Nigerian plant teams know: about 0.27 to 0.30 litres per kWh at good load. At 30 percent load that climbs towards 0.38 litres per kWh, a heat rate near 13,700 kJ/kWh and an efficiency around 26 percent. Part load costs fuel on any plant. Our piece on [how a gas turbine works](/blog/gas-turbine-how-it-works/) explains where the energy goes.

## What pushes gas turbine heat rate up

Compressor fouling is the big one. Dirt on the blades changes their shape and roughens the surface, so the compressor moves less air and needs more work to do it. Output falls and heat rate rises. Washing recovers most of it, but erosion doesn't wash out.

Ambient temperature is one you can only correct for. On a hot afternoon the air is less dense, the compressor swallows less mass flow, and output drops by something like half a percent per degree Celsius on many industrial machines. Gas turbine heat rate worsens too, more gently. Use your OEM's correction curves, not a rule of thumb.

Harmattan adds a second problem. Fine dust gets past imperfect filtration and fouls the compressor, and it loads up the inlet filters so the pressure drop across the house climbs. Every extra millimetre of water column of inlet loss is air density you've thrown away before the compressor sees it. We cover this in [harmattan dust and turbine derating](/blog/harmattan-dust-turbine-derating/), including why filter change-outs should follow differential pressure, not the calendar.

Hot gas path wear is slower but real. Worn seals, eroded blade tips and warped combustor liners all let energy go somewhere other than shaft power.

Part-load running is the one nobody can wash away. Most gas turbines are tuned for best efficiency near base load, and heat rate at 50 percent load can be noticeably worse. An oversized unit pays that penalty every hour.

## What pushes steam plant heat rate up

On a steam plant the turbine is only one contributor. A tired boiler gives a bad heat rate even if the turbine is spotless.

Condenser vacuum is the first place to look. If the vacuum is poor, because of tube fouling, air in-leakage, a weak cooling water supply or warm cooling water, the turbine exhausts at a higher pressure and extracts less work from every kilogram of steam.

Feedwater heaters come next. When a heater is bypassed or its tubes are leaking, the feedwater reaches the boiler colder than design, and the boiler burns more fuel to make up the difference. They're easy to leave out of service after a fault, because the plant keeps running.

Boiler excess air is the third. Too much air carries heat up the stack. Too little gives incomplete combustion and soot. Drifting oxygen trim, air heater leakage and dirty heat transfer surfaces all show up here, and stack temperature plus flue gas oxygen will tell you quickly.

Worn gland seals and stage deposits add to it. Our [thermal power plant explainer](/blog/thermal-power-plant-explained/) covers how the cycle fits together.

## How to track heat rate routinely

Honestly, most heat rate arguments turn out to be metering arguments.

Start with fuel. A fuel meter that reads 2 percent high makes a healthy machine look 2 percent worse, and one that reads low hides real deterioration. Gas needs flow measurement compensated for pressure and temperature, and a calorific value you actually know, from a gas analysis or chromatograph, not a figure copied off the supplier's first invoice. Liquid fuels need calibrated flow meters or consistent tank dips with temperature correction. Schedule meter calibration and keep the certificates with the heat rate record.

Output needs a trustworthy kWh meter at a defined point. Decide whether you're tracking gross or net, write it down, and don't change it.

Next, correct for conditions. A raw heat rate on a cool morning and a hot afternoon aren't comparable. Corrected heat rate adjusts the measured value back to reference ambient temperature, pressure, humidity, load and fuel properties, using the OEM correction curves or a plant model. Without it, your trend mostly shows the weather.

Then test under repeatable conditions. Pick a steady load, let the unit stabilise, log for a fixed period, and repeat it the same way each time. Trend the corrected figure monthly, and always test before and after a compressor wash and around every outage. The before-and-after pair shows what the wash or overhaul actually bought you.

Any compressor wash, meter calibration or inspection on live equipment needs isolation, lockout-tagout and a permit to work, and offline work means the unit shut down and cooled. When the figure moves, check the instrumentation before you dismantle anything.

If you want the numbers built into a wider plant review, a [power plant audit](/power-plant-audit-nigeria/) covers fuel metering and performance testing in one exercise.

Ready to find out where your fuel energy is going? Request a technical proposal or book a plant assessment through our [contact page](/#contact), and our engineers will set out a measurement plan for your units.

## Frequently Asked Questions

### What is a good heat rate for a power plant?

It depends on the technology. Small simple-cycle gas turbines typically sit around 10,000 to 14,000 kJ/kWh, steam plants roughly 9,500 to 11,000, and combined-cycle plants below 7,500. A good heat rate is one close to the plant's own design or test value, corrected to the same conditions.

### How do you convert heat rate to efficiency?

Divide 3,600 by the heat rate in kJ/kWh, or 3,412 by the heat rate in Btu/kWh. A heat rate of 12,000 kJ/kWh gives 3,600 / 12,000 = 0.30, which is 30 percent efficiency.

### Why do two sources quote different heat rates for the same plant?

Usually it's the basis. One figure might be gross and the other net of auxiliaries, or one on LHV and the other on HHV, which for natural gas differ by about 10 percent. Load, ambient conditions and fuel quality also move the number.

### How often should heat rate be checked?

A routine monthly corrected test works for most plants, plus a test before and after every compressor wash, overhaul or major repair. Continuous online calculation is better if your instrumentation supports it.

### Does a higher ambient temperature always worsen heat rate?

On a gas turbine, yes, though output falls faster than efficiency does. On a steam plant, warm cooling water raises condenser pressure and has a similar effect. Correct to reference conditions before blaming equipment for a seasonal change.
