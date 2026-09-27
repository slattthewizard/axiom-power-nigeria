---
meta_title: "Generator Not Producing Rated Power: Fault Diagnostics"
meta_description: "Generator not producing rated power? Diagnose fuel, air, cooling and control faults, run a proper load bank test and cost the repair before you buy new."
primary_keyword: "generator not producing rated power"
secondary_keywords: "generator low output causes, generator losing power under load, diesel generator derating, generator load bank test, generator kVA vs kW output"
---

# Generator Not Producing Rated Power: Fuel, Air, Cooling and Load Test Diagnostics

A 1,000 kVA prime set that trips its breaker at 640 kW is not a problem you can budget for next quarter. On a plant running continuous process load, a ceiling like that can cost several times the repair bill within a couple of weeks of lost throughput. When a generator is not producing rated power, the cause is rarely mysterious. It is fuel, air, cooling, the control and excitation side, or a derate you were always entitled to expect, and those can be separated in one instrumented day on site.

The expensive mistake is skipping diagnosis and going straight to a quotation for a new set. Plants have replaced healthy engines because nobody put a manometer on the turbo inlet.

## What your nameplate rating actually promises

Before you call anything a fault, establish what the set was rated to do. ISO 8528 defines rating classes that are not interchangeable. Emergency standby power carries no overload capability and assumes limited annual hours. Prime power permits variable load but assumes an average load factor well below peak, commonly around 70 percent over 24 hours. Continuous power is the only class supporting unlimited hours at fixed load.

A set sold as "500 kVA" may be 500 kVA standby and closer to 455 kVA prime. Run it as prime against the standby figure and it will look like a generator not producing rated power when it is simply being asked for output it was never sold with.

The second recurring confusion is kVA against kW. Standard alternator rating assumes 0.8 power factor, so 500 kVA delivers 400 kW of real power. A plant with heavy induction motors and poor power factor correction reaches the kVA limit while the engine is still coasting. That is a load-side problem, and the fix is correction plant, not an overhaul. Our [generator sizing guide](/blog/generator-sizing-guide/) covers setting that baseline at specification stage.

Third, verify the metering. A wrong current transformer ratio in the controller under-reports kW by exactly the ratio error, and checking it costs nothing.

If you are unsure which rating class and load profile your site needs, [request a technical proposal](/#contact) and we will scope an instrumented assessment before anyone quotes hardware.

## Fuel system: where a generator not producing rated power gives itself away

Fuel restriction is the most common single cause of low output on diesel sets in Nigerian service, and it presents the same way almost every time. The engine takes load smoothly to 50 or 60 percent, then frequency sags, black smoke appears, and it will not hold the next step.

Work through it in order, measuring rather than assuming:

- Supply restriction. Gauge fuel pressure before and after the primary and secondary filters at load, not at idle. An element that reads clean at no load will starve the engine at 80 percent.
- Water and contamination. Day tanks left half full through the rainy season grow microbial contamination at the fuel and water interface. Draw a bottom sample. If it is dark and stringy, the tank needs polishing, not another filter.
- Air ingress. A weeping union upstream of the lift pump will not leak diesel out but will draw air in, and the symptom is precisely a power ceiling under load.
- Injector condition. Coked or worn injectors cut delivery and spoil spray pattern. Bench testing a set is workshop work with proper equipment, not a field judgement.
- Pump and rack travel. On mechanically governed engines a sticking rack or a maladjusted maximum fuel stop caps output permanently. On electronic engines, read the fault codes and confirm whether the ECU is actively derating before touching anything mechanical.

Adulterated or low quality diesel also reduces energy content per litre and accelerates injector fouling. If specific fuel consumption has drifted upward at the same load, that shows in your cost per kWh well before it shows as a power complaint.

## Air, exhaust and cooling restrictions that quietly derate the set

A diesel engine makes power in proportion to the air mass it can get into the cylinder. Anything reducing air density or flow reduces output, and most of it is invisible from the control panel.

Measure inlet restriction with a manometer at the turbocharger inlet at full load. Many turbocharged engines specify a limit near 6 kPa, roughly 25 inches of water, but use the OEM figure for your model. A filter element clean in October can sit at the limit by January. Dust loading is a seasonal derating mechanism across the north and middle belt, and the same physics affects turbomachinery, as set out in [harmattan dust and turbine derating](/blog/harmattan-dust-turbine-derating/).

Then compare boost pressure against specification at rated speed and load. Low boost points to a fouled compressor wheel, a stuck wastegate, a leaking charge air cooler or boost pipe, or a turbine side carboned up from years of light loading.

Measure exhaust back pressure at the turbine outlet. Long runs, undersized pipework and silencers packed with soot all push back pressure past limits and the engine cannot scavenge. Typical limits fall between 3 and 7 kPa depending on engine family.

On the cooling side the failure modes are mundane and the effect is not. A blocked radiator core, internal scale, a failed thermostat, a slipping fan belt or a plant room with insufficient ventilation area all raise intake air and coolant temperature. Hot air recirculating in a poorly louvred room can lift intake temperature 10 to 15 degrees above ambient, and every degree costs air density.

Site derating is real and it is not a fault. Reference conditions under ISO 3046 assume roughly 25 degrees Celsius and 100 metres altitude. A site at 475 metres running at 41 degrees is legitimately down several percent before anything is wrong. Pull the manufacturer's derate curve before declaring a deficit. The standards catalogue is published by [ISO](https://www.iso.org/standards.html), and ISO 8528-1 and ISO 3046-1 are the two references worth keeping on file.

## Alternator, AVR and control-side causes of low generator output

If the engine holds speed and the fuel and air numbers are clean, the deficit is downstream of the crankshaft.

Voltage collapsing under load while frequency holds points at the excitation system. Check AVR sensing leads, the exciter stator and the rotating rectifier. A single failed diode will hold voltage at no load and drop it hard as soon as reactive load arrives, which reads on the panel as a set that cannot carry its rating.

Frequency sagging while voltage holds points back at the engine, governor or actuator linkage. On sets in parallel, check droop and load sharing settings before condemning either machine. Mismatched droop loads one set to its limit while the other idles.

Check the winding configuration too. A reconnectable alternator left in the wrong star or delta arrangement will not deliver rated current at the terminal voltage you expect. Insulation and winding resistance testing identifies a damaged stator, and a rewind is a workshop operation with a defined outage window, not a field repair.

Wet stacking is endemic on standby fleets. A set running for years at 15 to 20 percent load accumulates unburnt fuel and carbon in cylinders, exhaust and turbine housing, then cannot accept full load when it finally matters. The remedy is a controlled load bank exercise, and in advanced cases a top end clean.

## Load bank testing: proving the deficit before you spend

No credible repair scope should be signed without a load bank result. A stepped test at 25, 50, 75 and 100 percent, holding at least 30 to 60 minutes at full load, converts a vague complaint into a defensible number.

Record at every step: kW, kVA, power factor, phase voltages and currents, frequency, oil pressure, coolant and charge air temperature, boost, inlet restriction, exhaust back pressure and exhaust temperature per cylinder where instrumentation allows. Cylinder to cylinder exhaust spread alone will often identify a single failing injector.

One honest limitation. A purely resistive load bank proves the engine and cooling system but not the alternator's reactive capability. Where plant load is motor heavy, specify a reactive or combined bank so the excitation system is tested at realistic power factor. This needs proper equipment, a competent test engineer on site and a planned outage window.

**Hypothetical example: 1,000 kVA prime set, 800 kW prime rating.** Suppose the machine will not exceed roughly 640 kW. Instrumented running finds inlet restriction at 10.4 kPa against a 6.2 kPa limit, exhaust back pressure at 9.4 kPa and boost at 0.9 bar against 1.45 bar. The cause is a collapsed filter element plus a silencer heavily sooted from light loading. Filter housing repair, silencer replacement and a turbocharger exchange are a small fraction of what the lost output would cost over the same period.

**Hypothetical example: two 250 kVA standby sets in parallel.** One set sags to 47.6 Hz whenever a large block load engages. The engine is mechanically sound but has averaged 18 percent load for six years and is heavily wet stacked, with a fuel rack never reset after an earlier service. Staged load bank exercise, rack adjustment and injector refurbishment bring it back without a new set being required.

**Hypothetical example: 400 kVA set, 15 percent shortfall.** At 475 metres and a shed temperature of 41 degrees, the derate curve accounts for around 11 percent of it legitimately. The remainder can trace to a slipping fan belt and a radiator core packed with dust, both straightforward to correct. The balance is a sizing decision, not a fault.

To have your own deficit measured rather than estimated, [book a plant assessment](/#contact).

## Repair cost, downtime and the overhaul versus replace decision

Figures below assume a 500 kVA class diesel set in Nigerian service. Actual cost depends on engine family, whether parts are stocked locally or imported against lead time, condition found once the item is stripped, and site access. For a costed scope on your own set, see our [maintenance cost guide](/generator-turbine-maintenance-cost/) or [request a technical proposal](/#contact).

| Intervention | Typical scope | What drives the cost | Outage window |
|---|---|---|---|
| Instrumented diagnostic visit | Full load readings across fuel, air, exhaust, thermal | Instrumentation and engineer time on site | 1 day |
| Load bank test, stepped to 100% | 4 hours, resistive or combined | Bank rental, reactive vs resistive capability needed | 1 day |
| Fuel system service and tank polishing | Filters, separator, 5,000 L polish | Volume polished, contamination severity | 1 to 2 days |
| Injector refurbishment or replacement | 6 cylinder set, bench tested | Whether injectors are stocked or made to order, engine make | 2 to 3 days |
| Turbocharger overhaul or exchange | Including boost pipe and charge air cooler check | Exchange unit availability, import lead time | 2 to 4 days |
| Cooling system rebuild | Recore, thermostat, belts, ventilation correction | Radiator core availability, extent of corrosion found | 2 to 4 days |
| AVR and rotating rectifier replacement | With excitation testing | Part availability, whether the stator also needs work | 1 day |
| Top end engine overhaul | Heads, valves, injectors, timing | Condition at strip, parts sourcing, engine family | 7 to 14 days |
| Full overhaul plus alternator rewind | Engine and alternator, workshop | Scope found at strip, rewind materials, workshop lead time | 3 to 6 weeks |

The decision rule is straightforward. Where the deficit traces to fuel, air, cooling or controls, repair is almost always correct and pays back within one or two months of avoided downtime. Where compression is lost across several cylinders, alternator insulation has failed, or spares are no longer supported in country, the arithmetic shifts toward replacement and lead time becomes the governing risk. The same framework applies to larger rotating plant, set out in [turbine overhaul versus replacement](/blog/turbine-overhaul-vs-replacement/).

One caution on hybridisation. Solar or battery storage changes your fuel bill and run hours. It does not repair a derated set and it does not raise the block load the generator can accept. Solar reduces daytime energy demand, not the instantaneous starting load of a chiller or a crusher. Size any hybrid scheme around a generator proven on a load bank, not around the nameplate.

Structured servicing prevents most of this. Our [generator maintenance services](/generator-maintenance-nigeria/) cover scheduled intervals, fuel management and annual load testing, and a [power plant audit](/power-plant-audit-nigeria/) is the right starting point where several sets and a mixed load profile are involved. Captive generation is regulated by the [Nigerian Electricity Regulatory Commission](https://nerc.gov.ng/).

To scope the work on your own installation, [request a technical proposal](/#contact).

## Frequently Asked Questions

### How do I know if my generator is faulty or just correctly derated?

Pull the manufacturer's derate curve for your engine model and apply actual site altitude, intake air temperature and humidity. Compare that derated figure against measured full load output on a load bank. If the machine meets the derated number it is healthy and the problem is specification, not condition. If it falls short, you have a fault worth diagnosing.

### Can a generator lose power without any warning lights or alarms?

Yes, and it is common on mechanically governed engines with basic controllers. Gradual losses from air restriction, exhaust back pressure, injector wear and radiator fouling develop over months without crossing any alarm threshold. Only trend data or a stepped load test will reveal them, which is why annual load testing belongs in the maintenance schedule.

### How often should a standby generator be load tested?

Annual full load testing is the accepted minimum for standby sets, with shorter exercise runs monthly. Sets that habitually run below 30 percent load need load bank exercise more often to control wet stacking. Sites with critical loads, such as hospitals and data rooms, should test on a defined schedule and retain the recorded results.

### Will servicing the generator restore full rated output?

It depends on the cause. Fuel, air, cooling and control faults usually respond fully to corrective work and the set returns to rating. Mechanical wear such as lost compression, worn liners or a failed alternator winding will not be recovered by servicing and needs an overhaul with a planned outage window and a qualified engineer on site. The instrumented test tells you which category you are in before you commit budget.
