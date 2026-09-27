---
meta_title: "Megger Test & Insulation Resistance: A Plant Guide (Nigeria)"
meta_description: "How a megger test measures insulation resistance on motors, test voltage by rating, PI and DAR, temperature correction and safe isolation for Nigerian plants."
primary_keyword: "megger test"
secondary_keywords: "insulation resistance test, megger test for motor, polarization index, insulation resistance values"
---

# Megger Test and Insulation Resistance: What Plant Engineers Need to Know

A motor that trips on earth fault, or a feeder that fails an acceptance check before commissioning, usually sends the maintenance team reaching for a megger. A megger test applies a DC voltage across a winding's insulation and measures the resistance to earth or between phases, and the reading tells you how much moisture, contamination or ageing damage has crept into the insulation before it becomes an outage.

For plant managers and maintenance engineers running motors, generators, transformers and switchgear in Lagos, Port Harcourt, Kaduna or Warri, insulation resistance testing is one of the few checks that catches deterioration before it trips a breaker or, worse, puts a technician near a faulted winding. The test itself is simple to run. Interpreting the number correctly, and doing it safely, is where most sites go wrong.

This article covers what the test measures, how to pick a test voltage by equipment rating, what polarization index and dielectric absorption ratio add on top of a single reading, how temperature changes the number, and the isolation steps a permit to work should always cover.

## What a Megger Test Actually Measures

Insulation is not a perfect barrier. Under a DC voltage, a small current leaks through the insulation to earth or between windings, and Ohm's law converts that leakage current into a resistance reading, usually in megohms. A healthy, dry winding presents a high resistance path. A winding with absorbed moisture, carbon tracking, or embedded conductive dust presents a lower one, because the contamination gives the leakage current an easier route.

The reading is a screening test, not a proof of soundness. It tells you whether the insulation is dry and clean enough to be put into service or kept in service. It does not tell you the condition of bearings, the state of the rotor, or whether the winding will survive a full-voltage surge. For that level of confidence, insulation resistance is read alongside other checks such as winding resistance, vibration and, where the machine's history calls for it, a surge or hipot test carried out by qualified personnel with the right equipment.

## Running a Megger Test: Matching Test Voltage to the Machine

The DC test voltage applied has to suit the winding's rated voltage, not the tester's maximum output. IEEE Standard 43 gives guidance on this: windings rated below 1 kV are typically tested at 500 V DC, with the reading taken and recorded at 60 seconds. Mid-voltage windings usually take a higher test voltage in the 500 V to 1,000 V DC range, and windings rated above 12 kV can call for test voltages up to 10,000 V DC. The exact step for a given machine sits in the standard's voltage table and in the test set manufacturer's instructions, so the correct approach is to match the instrument setting to the equipment nameplate rather than defaulting to whatever voltage the megger was last left on.

Applying too low a voltage understates the stress the insulation will actually see in service and can miss a weak spot. Applying too high a voltage on old or already-degraded insulation risks damaging it further during the test itself, which is why the nameplate rating, not habit, should set the dial.

A single spot reading, taken once and filed away, only tells you whether the winding passes or fails against a minimum threshold on that day. A commonly used minimum is the "kV plus 1" rule: insulation resistance, corrected to a reference temperature, should be at least 1 megohm per kV of the winding's rated voltage, plus 1 megohm. On a 400 V motor, for example, that works out to a minimum of roughly 1.4 megohms, though most healthy low-voltage motors in good condition read into the hundreds or thousands of megohms, and a reading only just clearing the minimum is itself a warning sign worth investigating rather than a pass to file away.

## Polarization Index and Dielectric Absorption Ratio

A single one-minute reading is useful, but trending the reading over time within the same test gives a clearer picture, because it separates a winding that is genuinely dry and sound from one that is merely warm or briefly stable.

Two ratios are used for this:

- Dielectric absorption ratio (DAR): the insulation resistance at 60 seconds divided by the reading at 30 seconds.
- Polarization index (PI): the insulation resistance at 10 minutes divided by the reading at 1 minute.

A sound, dry winding keeps absorbing charge and its resistance reading keeps climbing through the test, so the ratio comes out well above 1.0. A contaminated or moisture-laden winding reaches a stable leakage current quickly, so the ratio sits close to 1.0 or below it. PI is the ratio most commonly specified because it is less sensitive to test-lead capacitance and instrument variation than DAR, and it is the ratio IEEE 43 gives minimum values for by insulation class.

| Insulation class | Minimum acceptable polarization index |
|---|---|
| Class A | 1.5 |
| Class B | 2.0 |
| Class F | 2.0 |
| Class H | 2.0 |

Take a hypothetical 415 V, 75 kW induction motor pulled from standby storage after the rainy season. A one-minute spot reading alone might look acceptable, comfortably above the kV-plus-1 minimum. But if the 10-minute reading barely rises above the 1-minute reading, the PI comes out near 1.0, which points to trapped moisture even though the spot reading passed. That motor is a candidate for drying out and retesting before it goes back into service, not for a straight return to the panel on the strength of one number.

## Temperature Correction: Comparing Readings Fairly

Insulation resistance falls as winding temperature rises, and it falls sharply: as a rule of thumb drawn from IEEE 43 guidance, resistance roughly halves for every 10°C the winding is above a 40°C reference temperature, and roughly doubles for every 10°C it is below that reference. A reading taken on a motor at 25°C ambient during Harmattan season and a reading taken on the same motor at 38°C ambient in the wet season are not directly comparable until both are corrected to the same reference temperature, usually 40°C.

Skipping this step is one of the most common reasons a maintenance log shows insulation resistance "falling" year on year when the winding has not actually degraded, or "improving" when it has. Record the winding temperature (not just ambient air temperature) at the time of test, and apply the correction before comparing today's number against last year's baseline.

## Interpreting a Falling Trend

A single low reading, on its own, tells you the winding needs attention before it is energised. A trend of readings falling test after test, even while each one individually clears the minimum, is the more useful signal, because it shows the insulation losing margin over time rather than being marginal at a single point.

Common causes on Nigerian sites include ingress of moisture during long shutdowns, dust and carbon build-up on winding surfaces in dusty environments, and oil or fuel contamination near engine-driven generator sets. A stable low reading that does not respond to drying out points to physical damage to the insulation itself rather than surface contamination, and that distinction changes whether the fix is cleaning and drying or a rewind. Our companion article on [motor rewinding](/blog/electric-motor-rewinding/) covers how that decision gets made once insulation testing has ruled contamination in or out.

## Safety and Isolation Before Testing

A megger test injects a DC voltage into equipment that is normally isolated for the purpose, and the winding itself can retain a charge after the test that is dangerous if not discharged. This work needs qualified personnel operating under a permit to work, with the circuit isolated and locked out before any test lead is connected, and with the winding discharged to earth after the test before it is touched or reconnected. This article does not cover the connection sequence in enough detail to let someone without that training carry it out, and it should not be read as a substitute for that training or for the test set manufacturer's procedure.

Before any insulation resistance test on a motor, generator or transformer winding, confirm:

- The circuit is fully isolated, tagged and proved dead at the test points.
- All other personnel are clear of the equipment and warned that a test is in progress.
- The correct test voltage for the equipment's rated voltage has been selected on the instrument.
- A discharge procedure is ready to run immediately after the test, before any lead is disconnected by hand.

Getting a insulation resistance test wrong on a large machine, or skipping the discharge step, is not a minor process error. It is a shock and arc-flash hazard, which is why this sits with engineers who hold the relevant electrical competence rather than with whoever is nearest the panel.

Where a reading comes back marginal or a PI trend is falling, the next step is usually a wider look at the machine rather than a single repeat test. Our team can assess a motor, generator or transformer winding as part of a broader rotating equipment inspection: see our [rotating equipment and compressor services](/rotating-equipment-services-nigeria/) page for what that covers, or [request a technical proposal](/#contact) if you want a scoped assessment for a specific machine or fleet.

## Frequently Asked Questions

### What test voltage should I use for a megger test on a low-voltage motor?

For windings rated below 1 kV, IEEE 43 guidance points to a 500 V DC test voltage, with the one-minute reading as the reference point. The test set should always be set to match the equipment's nameplate voltage rating rather than left on a default setting, and the manufacturer's instructions for the specific instrument take precedence over any general rule.

### What counts as a good insulation resistance reading for an industrial motor?

There is no single pass number that applies to every machine. A widely used minimum is roughly 1 megohm per kV of rated voltage plus 1 megohm, corrected to a 40°C reference temperature, but a healthy low-voltage motor in good condition typically reads far above that minimum. A reading that only just clears the minimum is worth investigating even though it technically passes.

### What is the difference between polarization index and dielectric absorption ratio?

Both compare how the insulation resistance reading climbs over time during a single test. Dielectric absorption ratio divides the 60-second reading by the 30-second reading, while polarization index divides the 10-minute reading by the 1-minute reading. Polarization index is the ratio most standards and specifications set a minimum value for, and it is less affected by test-lead and instrument variation than the shorter dielectric absorption ratio.

### How often should insulation resistance testing be done on plant motors and generators?

The right interval depends on the machine's criticality, its operating environment and its maintenance history, and the OEM manual for the specific machine should be the starting point rather than a generic figure. Many sites include a megger test at scheduled shutdowns, after a long idle period, and after any event that could have exposed the winding to moisture, flooding or heavy contamination.

### Can insulation resistance testing be done while the motor is still connected to the switchboard?

No. The circuit needs to be fully isolated from all sources of supply, locked out and proved dead before any test lead is connected, because the test itself applies a voltage that must not reach other equipment or personnel, and any capacitors or cabling connected to the winding must be accounted for before the test starts. This isolation and the post-test discharge should be carried out by personnel qualified for electrical work under a proper permit to work.
