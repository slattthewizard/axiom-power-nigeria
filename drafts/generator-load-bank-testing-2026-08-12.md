---
meta_title: "Generator Load Bank Testing: How to Specify Acceptance Tests"
meta_description: "Generator load bank testing in Nigeria: what an acceptance test proves, resistive versus reactive load banks, site derating and realistic NGN test costs."
primary_keyword: "generator load bank testing"
secondary_keywords: "load bank test generator, generator acceptance testing, resistive load bank, generator commissioning test Nigeria, standby generator load test"
---

# Generator Load Bank Testing: Why Acceptance Tests Matter and How to Specify Them

A 220-bed private hospital in Lagos took delivery of an 800 kVA standby set, watched it idle for twenty minutes in the plant room, signed the handover certificate and released the final 30 per cent payment. Fourteen months later a grid outage put theatre, imaging and the chiller plant on that machine for the first time. It held for nine minutes and then shut down on high coolant temperature at roughly 68 per cent load. Generator load bank testing at handover would have exposed that fault inside the first hour of the first day, while the supplier still had money outstanding and a contractual reason to fix it.

Instead the hospital paid NGN 11.4 million (about USD 7,400) for a radiator core, a new fan drive and revised plant room ventilation, and carried the cost of an unplanned theatre shutdown. The set was never faulty on paper. It was simply never asked to do the job it was bought for.

## What a Generator Load Bank Test Actually Proves, and What It Does Not

A load bank is a controlled, adjustable artificial load. You connect it to the generator terminals or to the downstream busbar, dial in load in defined steps, and hold each step long enough for the machine to reach thermal equilibrium while you record what it does.

The point is not to see whether the set starts. Every set starts. The point is to make the machine reveal the faults that only appear under sustained heat and current.

A properly run test will find a cooling package undersized for the plant room, an alternator that overheats above 70 per cent load, an AVR that hunts under inductive load, injectors that smoke past 80 per cent, a fuel line that starves the engine at full rate, exhaust back pressure outside the manufacturer's limit, and a governor that cannot hold frequency through a block load step. None of these announce themselves during a no-load run.

One limit is worth stating plainly. A load bank at the generator terminals tests the generator, not your distribution, so it proves nothing about your changeover panel, cable sizing, earth fault protection or ATS transfer timing. Where switchgear allows, connect downstream of the transfer switch so the test covers the path the real load takes.

If you are at the point of accepting a new set or taking over an existing installation, [request a technical proposal](/#contact) for a witnessed acceptance test before the retention money is released. The commercial leverage disappears the day you sign.

## Resistive, Reactive and Resistive-Reactive Load Banks

Most load bank hire in Nigeria is resistive only, because resistive banks are cheaper, simpler and more widely available. That matters, because a resistive bank tests half the machine.

A resistive load bank draws current at unity power factor. It loads the engine to full kW and heats the alternator windings, but it never asks the excitation system to supply reactive current. Your 1,000 kVA set is rated at 0.8 power factor, which is 800 kW. Load it to 800 kW resistive and the engine is at 100 per cent while the alternator sits at 800 kVA out of 1,000, with the AVR barely working.

Real industrial load is inductive. Motors, transformers, welding sets and lightly loaded drives all draw magnetising current, and the failure modes that appear under reactive load are excitation-related: AVR instability, voltage hunting, overexcitation shutdown and rotating diode weakness.

A resistive-reactive load bank adds inductive elements so you can set 0.8 power factor lagging and load engine and alternator to their full ratings at once. For a hospital, a data facility, a bottling plant or anything with heavy motor content, that is the test that matters.

A beverage bottling plant in Ogun State learned this on a 1,250 kVA prime set. The handover test was resistive only and passed cleanly at 1,000 kW. When the filler hall and the ammonia compressors came on together, terminal voltage oscillated between 388 V and 428 V at about 1.5 Hz and the drives began tripping on DC bus overvoltage. The fault was AVR stability gain set for a factory test load and never tuned for a lagging site load. Two days of engineering, a resistive-reactive bank and a retune cost NGN 3.8 million (about USD 2,450), against six weeks of intermittent production losses before the cause was isolated.

## Specifying the Acceptance Test: The Schedule to Write Into Your Purchase Order

Do not accept "load tested" as a line item. Specify the schedule, the instrumentation, the pass criteria and who witnesses it, and make final payment conditional on the report.

A defensible acceptance schedule for a new set looks like this:

- Pre-test checks: oil and coolant levels, fuel quality and quantity for the full test, exhaust back pressure, battery condition, ventilation openings clear
- Staged load: 30 minutes at 25 per cent, 30 minutes at 50 per cent, 60 minutes at 75 per cent, then 120 to 240 minutes at 100 per cent of site rating
- Readings every 15 minutes: kW, kVA, power factor, all three line voltages and currents, frequency, oil pressure, coolant temperature, exhaust gas temperature per cylinder, ambient and plant room temperature
- Block load acceptance: a single step to the largest expected load step, recording voltage dip, frequency dip and recovery time
- Load rejection: full load to zero in one step, recording voltage and frequency overshoot and settling time
- Sustained full load last, not first, so the machine is thermally soaked when it is worked hardest

Pass criteria come from the performance class you specified. [ISO 8528-1](https://www.iso.org/standard/68539.html) defines the rating duty classes, and the series sets performance classes G1 to G4 fixing the permitted steady state and transient voltage and frequency bands. A supplier who cannot tell you which class the set was built to has not read the specification either.

Record cylinder exhaust temperature deviation, not just the average. A spread beyond the engine maker's limit at full load points at injector or valve problems that will surface as a failure six months later.

Two things here are non-negotiable. The work needs an outage window, because you cannot load bank a set while it carries live plant load. It also needs a qualified engineer on site with the right cables and connection method, because a 1,000 kW resistive bank rejects a megawatt of hot air and will recirculate into the radiator or engine intake if sited badly, invalidating every temperature reading you take. Talk it through before you book the window on [+234 803 000 0000](tel:+2348030000000).

## Site Derating: Why the Factory Test Certificate Is Not Your Rating

The certificate in the document pack was produced at standard reference conditions, near 25 degrees C, close to sea level and at moderate humidity. Very little of Nigeria looks like that, and the plant room usually looks worse than the site.

Ambient temperature and altitude both reduce available output. The engine maker's derating curve governs and the numbers vary by engine family, but as an order of magnitude expect a few per cent lost per 300 m of altitude above the reference and a few per cent per 5 degrees C of ambient above it, with turbocharged aftercooled engines generally less sensitive.

So a set stamped 1,000 kVA may be a 900 kVA machine in a Lagos plant room at 42 degrees C intake, and lower again on the Jos plateau. Testing at 100 per cent of nameplate in those conditions is not conservative, it is unrealistic, and it will fail a healthy machine.

Fix the site rating first, in writing, using the manufacturer's curve and the measured plant room intake temperature, then test to that number. Measure intake air at the machine, not outside the building. The gap between the two is frequently 8 to 12 degrees C where ventilation is marginal, and it is capacity you have already paid for.

If nobody has established the true site rating of your installed fleet, a [power plant audit](/power-plant-audit-nigeria/) is the cheaper starting point, and it usually pairs well with a review of your [generator sizing](/blog/generator-sizing-guide/) assumptions.

## Periodic Load Bank Testing for Standby Sets and the Wet Stacking Problem

Acceptance testing is a one-off. Standby sets need periodic proof too, and for a different reason.

Standby machines in Nigeria are often exercised weekly off load or on a token load for twenty minutes. A diesel engine running below roughly 30 per cent of rating never reaches design cylinder temperature. Unburnt fuel and lube oil accumulate in the combustion chamber, exhaust ports, turbocharger and exhaust system. That is [wet stacking](/blog/diesel-generator-wet-stacking/), and it degrades output, glazes bores and eventually requires intrusive repair.

[NFPA 110](https://www.nfpa.org/codes-and-standards/nfpa-110-standard-development/110) is a United States standard and not Nigerian law, but it is the benchmark most insurers, hospital accreditation bodies and international consultants reference. Its logic is worth borrowing: exercise monthly at not less than 30 per cent of nameplate kW or to the manufacturer's minimum exhaust gas temperature, and where the monthly exercise cannot achieve that, run an annual supplemental load bank test in stages. Check the edition your insurer cites before writing it into a contract.

A telecoms switching facility in Abuja ran a 500 kVA standby set at a measured 11 per cent load factor for three years on weekly off load exercise. By the third year it smoked heavily on start, output had fallen and a turbocharger was passing oil. Cleaning, injector replacement, turbo overhaul and a corrective load bank burn came to NGN 9.6 million (about USD 6,200). Three annual 4-hour staged tests would have cost roughly NGN 5.4 million in total and kept the machine in condition.

Where a site genuinely runs a low load factor, the answer is not more exercise runs at low load. It is a permanently installed load bank, a resized set, or a maintenance regime that accepts the condition and plans for it. That decision belongs in a written [generator maintenance](/generator-maintenance-nigeria/) scope, not in an operator's diary.

## What Generator Load Bank Testing Costs in Nigeria

Costs move with diesel price, mobilisation distance and load bank availability, and reactive banks carry a premium because there are fewer of them in country. The figures below are indicative day rates for planning and assume Lagos or Port Harcourt mobilisation. Confirm against a written quotation.

| Item | Capacity | Indicative cost (NGN) | USD equivalent | What it covers |
| --- | --- | --- | --- | --- |
| Resistive load bank hire | 300 kW | 350,000 to 550,000 per day | 225 to 355 | Engine kW loading, cooling and exhaust proof |
| Resistive load bank hire | 1,000 kW | 950,000 to 1,500,000 per day | 615 to 970 | As above, large sets |
| Resistive-reactive bank hire | 500 kVA at 0.8 pf | 1,100,000 to 1,800,000 per day | 710 to 1,160 | Adds AVR, excitation and rotating diode proof |
| Test engineer and instrumentation | 2 days | 600,000 to 900,000 | 385 to 580 | Witnessed readings, block load, written report |
| Cabling, mobilisation, siting | Per visit | 350,000 to 700,000 | 225 to 450 | Connection, heat rejection siting, safety |
| Diesel for an 8-hour staged test | 1,000 kVA set | About 1,350,000 | About 870 | Roughly 1,080 litres at prevailing AGO price |

A full witnessed acceptance test on a 1,000 kVA set, resistive-reactive, with report, typically lands between NGN 4.5 million and NGN 6 million (about USD 2,900 to USD 3,900). Set that against a machine costing NGN 130 million or more, and against the [cost of an hour of unplanned downtime](/blog/plant-downtime-cost-per-hour/) in your plant, and the arithmetic is not close.

The test also buys a baseline. Fuel consumption per kWh, temperature rise at each load step and voltage regulation at commissioning become the reference for every future test. Without one, a degrading machine looks normal because nobody knows what normal was.

To scope an acceptance test, a periodic programme or a fleet baseline, [book a plant assessment](/#contact) and we will size the load bank, the outage window and the schedule to your equipment.

## Frequently Asked Questions

### How long should a generator load bank test run?

For acceptance testing, plan a minimum of four hours staged at 25, 50, 75 and 100 per cent of the site rating, with the longest period at full load and taken last. Shorter tests do not allow the cooling system, alternator windings and exhaust system to reach thermal equilibrium, which is exactly where most faults appear. For periodic testing of a standby set that runs at low load factor, two to four hours at rising load is generally sufficient. The engine manufacturer's guidance takes precedence over any general rule.

### Can I load test using the building load instead of a load bank?

Sometimes, and it is valid if the building load reaches the required percentage of rating and holds steady long enough. The problems are that most sites cannot reach 75 to 100 per cent on demand, the load varies so readings are not comparable, and you cannot perform controlled block load or load rejection steps. Building load testing also puts live plant at risk if the set fails mid-test. Use it for routine exercise, and a load bank for acceptance and annual proof.

### Does load bank testing damage the generator?

No. A correctly run test loads the machine within its rating and within the manufacturer's temperature and pressure limits, which is the duty it was designed for. Damage risk comes from bad practice, not from loading: siting the bank so hot discharge air recirculates into the radiator, undersized cables, testing beyond the derated site rating, or running a machine with a pre-existing fault to destruction. That is why the pre-test checks and a qualified engineer on site matter.

### Should we specify a resistive or a resistive-reactive load bank?

If the plant load is predominantly motors, compressors, transformers or drives, specify resistive-reactive at 0.8 power factor lagging so the alternator and excitation system are tested at full kVA. If the load is genuinely close to unity power factor, a resistive bank is defensible and cheaper. For acceptance testing of any new set above roughly 250 kVA, resistive-reactive is the safer specification because it is the only way to prove the AVR and rotating diodes under realistic conditions. Note that reactive banks are less widely available in Nigeria, so book the outage window around equipment availability.
