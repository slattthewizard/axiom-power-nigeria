---
title: "kVA to kW Conversion: A Working Guide for Sizing Industrial Generators in Nigeria"
navTitle: "kVA to kW Conversion: A"
metaTitle: "kVA to kW Conversion for Generator Sizing in Nigeria"
metaDescription: "kVA to kW conversion for generator sizing in Nigeria: the formula, why sets are rated at 0.8 power factor, worked examples and sizing mistakes to avoid."
primaryKeyword: "kva to kw"
secondaryKeywords: "kw to kva, kva calculator, kw vs kva, generator kva rating"
publishedDate: "2026-10-06"
tag: "Generators"
subtitle: "A generator nameplate says 500 kVA. The load schedule from the electrical consultant is in kW. Procurement needs a single number to compare quotes, and nobody on the call agrees on the multiplier."
canonical: "https://axiompowerng.com/blog/kva-to-kw-conversion/"
faq:
  - question: "Is kVA the same as kW?"
    answer: "No. kVA is apparent power, the figure an alternator's windings and cabling are rated to carry. kW is real power, the portion that does actual work. They are equal only at unity power factor, which is rare on a real industrial load, so a genset's kVA figure is always equal to or larger than its kW output."
  - question: "What power factor should I use if the datasheet does not state one?"
    answer: "0.8 lagging is the standard default for industrial diesel and gas gensets and is a reasonable assumption when nothing else is given. It should not be treated as universal: some alternator designs and most modern gas gensets carry a different nameplate pf, so the specific OEM datasheet always takes precedence over the default."
  - question: "How do I convert kVA to amps for cable sizing?"
    answer: "For a balanced three-phase supply, current equals kVA multiplied by 1,000, divided by the line voltage multiplied by the square root of three. The line voltage used must match the actual site supply, and the resulting figure is one input into cable and breaker selection, which should be finalised by a qualified electrical engineer against the specific installation."
  - question: "Why does my 500 kVA generator not deliver 500 kW?"
    answer: "Because 500 kVA is the apparent power limit of the alternator, not the real power output. At the standard 0.8 power factor, a 500 kVA set delivers around 400 kW. The remaining gap is reactive power, which the alternator still has to carry in current terms even though it does no useful work at the load."
  - question: "Does a low site power factor mean I need a bigger generator?"
    answer: "It can. A lower power factor than the 0.8 the set is rated against means more current is needed to deliver the same real kW, which can push the alternator toward its kVA limit before the engine reaches its kW limit. Correcting the site's power factor, or specifying the genset against the actual measured pf rather than the 0.8 default, avoids over-buying kVA to compensate."
---
A generator nameplate says 500 kVA. The load schedule from the electrical consultant is in kW. Procurement needs a single number to compare quotes, and nobody on the call agrees on the multiplier. This mix-up between kVA and kW is one of the more common ways a plant ends up with a genset that trips on load, runs hot, or simply cannot carry the motors it was bought for.

The conversion itself is short: kW equals kVA multiplied by power factor. The complications sit around that one line: which power factor to use, why the generator industry settled on 0.8 as the default, and what the number means once you add three-phase current, derating and a mixed motor load into the picture. This guide works through the maths a plant manager, procurement officer or facility engineer actually needs when reading a genset datasheet or comparing kVA to kW across supplier quotes.

## kVA to kW: the formula

kVA (kilovolt-amperes) is apparent power: what the alternator's windings and insulation are built to carry, regardless of how efficiently that power turns into work. kW (kilowatts) is real power: the part that actually turns a shaft, lights a bulb or spins a motor. The link between them is the power factor (pf), a number between 0 and 1 that describes how far the current lags the voltage on an inductive load.

The formula for a genset, using its nameplate pf:

kW = kVA x pf

So a set rated 500 kVA at 0.8 pf delivers 500 x 0.8 = 400 kW of real power. That 400 kW is the number that matters for comparing a generator against a load schedule expressed in kW, or against a grid supply also expressed in kW. The kVA figure alone tells you what the alternator and cabling must be rated for; it does not tell you how much work the set can actually do.

## Why generators are rated in kVA, not kW

A generator's nameplate leads with kVA because the alternator's physical limit is current and voltage, not the power factor of whatever gets plugged into it. The windings, insulation and cooling are sized to a maximum current at a given voltage; that ceiling is fixed however the load behaves. The engine driving the alternator has a separate limit: the horsepower it can deliver continuously. Power factor is the bridge between the two.

The industry default of 0.8 lagging is not arbitrary. Most industrial and commercial loads, motors, transformers, fluorescent and LED drivers, are inductive and tend to sit around 0.8 pf in normal service. Rating the alternator at 0.8 pf lets the manufacturer quote the largest kVA figure the windings will tolerate while sizing the engine to match the kW that a typical inductive load mix will actually draw. Push the same alternator to run at a lower (worse) power factor and the current for a given kW rises, which is why an unusually low site power factor can force a bigger genset than the kW load alone would suggest. Run it at unity pf (a resistive-only load, rare on an industrial site) and the same alternator can often deliver its full kVA figure as kW, engine permitting.

This matters when a spec sheet only gives kVA: unless the pf is stated, 0.8 is the safe assumption for an industrial diesel or gas genset, but the OEM datasheet for the specific model is what governs the actual figure, not a rule of thumb.

## kW to kVA: converting the other direction

Where the load is known in kW, usually because it comes from an electrical load schedule or an existing grid bill, and the question is what size of genset to specify, the formula rearranges to:

kVA = kW / pf

A load schedule totalling 350 kW, assumed at 0.8 pf, needs a genset rated at 350 / 0.8 = 437.5 kVA at minimum, before adding margin for starting currents, future load and derating (see the derating note below). This is the arithmetic behind most of the entries in a generator sizing exercise; the harder part is usually building an honest load schedule and starting-current allowance, which /blog/generator-sizing-guide/ covers in more detail.

## Worked examples: three genset ratings converted

These are illustrative calculations only, not equipment recommendations for any particular site. All three assume the standard 0.8 lagging power factor; a datasheet stating a different pf should be used in its place.

| Rating given | Power factor | Calculation | Result |
|---|---|---|---|
| 250 kVA (genset nameplate) | 0.8 | 250 x 0.8 | 200 kW |
| 500 kVA (genset nameplate) | 0.8 | 500 x 0.8 | 400 kW |
| 320 kW (load schedule) | 0.8 (assumed) | 320 / 0.8 | 400 kVA minimum |

Take a hypothetical facility with a load schedule of 320 kW at an assumed 0.8 pf. The bare-minimum genset rating is 400 kVA, but that figure has no allowance for motor starting current, harmonic loads from variable frequency drives, or headroom for a future load addition. In practice the set actually specified would sit above that minimum once those factors are applied, which is a separate sizing exercise from the kVA to kW conversion itself.

## Getting three-phase current from a kVA rating

Once a kVA figure is settled, the next number most electricians and panel designers need is current, for cable sizing, breaker selection and switchgear rating. For a balanced three-phase system:

I = (kVA x 1,000) / (V x root 3)

where V is the line-to-line voltage. Nigerian industrial and commercial three-phase supply is commonly quoted around 415V line-to-line (with some sites now specifying the IEC-harmonised 400V figure); the OEM or switchgear datasheet for the specific installation governs which figure to use.

Worked at 415V: a 500 kVA set gives I = (500 x 1,000) / (415 x 1.732), which comes to roughly 696 amps of full-load line current. That figure feeds directly into cable and breaker selection, which is not a calculation to do from a rule of thumb alone; it needs a qualified electrical engineer working from the actual site voltage, cable run and protection scheme.

## Common sizing mistakes when working from a kVA rating

A handful of errors show up repeatedly when a kVA figure gets converted or compared without enough care:

- Assuming 0.8 pf when the OEM datasheet states a different figure for that specific alternator, particularly on gas gensets and some newer alternator designs.
- Comparing a genset's kVA nameplate directly against a load schedule in kW, without converting either figure to the same unit first.
- Ignoring motor starting current (which can be several times running current) and sizing purely to the steady-state kW total.
- Treating the standby kVA rating on a datasheet as usable continuously, when the same set carries a lower prime or continuous rating for sustained duty. ISO 8528 rating classes cover this distinction and it is a common source of undersizing when a standby-rated set is run as the primary source.
- Skipping altitude and ambient temperature derating on the engine, which reduces the usable kW even though the alternator's kVA rating on paper stays the same. This bites harder in the harmattan season in the northern hubs than in Lagos or Port Harcourt.
- Applying a blanket derating percentage instead of checking the manufacturer's specific derating curve for the model and site conditions.

Any one of these on its own can leave a set that looks correctly rated on paper but trips on load, runs permanently overloaded, or fails to start large motors reliably. Getting this stage right is largely why a proper sizing exercise takes a load schedule and a site visit rather than a single kVA number.

## Where the conversion fits into a full sizing decision

The kVA to kW conversion is one input into a sizing decision, not the whole of it. A full sizing exercise also weighs starting currents, harmonic loads from drives and UPS systems, future expansion, fuel type, and the standby-versus-prime rating question covered above. /blog/generator-sizing-guide/ works through that fuller process, and /blog/power-factor-explained/ covers what drives a site's actual power factor away from the 0.8 assumption in the first place, which matters once the genset is running real loads rather than a nameplate figure.

Where the load schedule is uncertain, the existing generator is undersized, or a facility is choosing between kVA ratings from different suppliers, a site assessment settles the numbers against the actual equipment rather than assumptions. Our engineers can review a load schedule and existing switchgear and set out what rating actually fits the site: request a technical proposal at /#contact, or read more on /generator-maintenance-nigeria/ for what an ongoing maintenance scope covers once the set is sized and running.

## Frequently Asked Questions

### Is kVA the same as kW?

No. kVA is apparent power, the figure an alternator's windings and cabling are rated to carry. kW is real power, the portion that does actual work. They are equal only at unity power factor, which is rare on a real industrial load, so a genset's kVA figure is always equal to or larger than its kW output.

### What power factor should I use if the datasheet does not state one?

0.8 lagging is the standard default for industrial diesel and gas gensets and is a reasonable assumption when nothing else is given. It should not be treated as universal: some alternator designs and most modern gas gensets carry a different nameplate pf, so the specific OEM datasheet always takes precedence over the default.

### How do I convert kVA to amps for cable sizing?

For a balanced three-phase supply, current equals kVA multiplied by 1,000, divided by the line voltage multiplied by the square root of three. The line voltage used must match the actual site supply, and the resulting figure is one input into cable and breaker selection, which should be finalised by a qualified electrical engineer against the specific installation.

### Why does my 500 kVA generator not deliver 500 kW?

Because 500 kVA is the apparent power limit of the alternator, not the real power output. At the standard 0.8 power factor, a 500 kVA set delivers around 400 kW. The remaining gap is reactive power, which the alternator still has to carry in current terms even though it does no useful work at the load.

### Does a low site power factor mean I need a bigger generator?

It can. A lower power factor than the 0.8 the set is rated against means more current is needed to deliver the same real kW, which can push the alternator toward its kVA limit before the engine reaches its kW limit. Correcting the site's power factor, or specifying the genset against the actual measured pf rather than the 0.8 default, avoids over-buying kVA to compensate.
