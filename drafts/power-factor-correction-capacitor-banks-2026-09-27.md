---
meta_title: "Power Factor Correction & Capacitor Banks in Nigeria"
meta_description: "Fixed vs automatic capacitor banks in Nigeria: correction options, harmonic detuning and the generator AVR risk of over-correcting power factor."
primary_keyword: "power factor correction"
secondary_keywords: "capacitor bank, automatic power factor correction panel, apfc panel, detuned capacitor bank, leading power factor"
---

# Power Factor Correction and Capacitor Banks: What a Plant Manager Needs to Get Right

If the utility bill or the generator load report keeps showing a lagging power factor below 0.85, correction is usually the right move, but it is easy to size a capacitor bank for the wrong problem. Power factor correction fixes the reactive current drawn by induction motors, welding sets, lighting ballasts and variable frequency drives. It does not fix a harmonic-rich supply, and on a site running its own generators, an oversized or badly tuned bank can push the power factor the wrong way and unsettle the automatic voltage regulator (AVR).

This is written for the person who has to decide between a fixed bank, an automatic power factor correction (APFC) panel and a detuned bank, and who needs to know what happens once it is installed, not just what it costs to buy. Pricing moves with exchange rates and panel specification, so it is not covered here: a scoped quote comes from a site survey against your actual load and harmonic profile.

## Why Low Power Factor Is a Problem Worth Fixing

Power factor is the ratio of real power (kW), the power that does work, to apparent power (kVA), the power the supply or the generator has to deliver. A plant with a lot of lightly loaded induction motors, fluorescent or old-style discharge lighting, and welding load typically sits between 0.6 and 0.8 lagging. Every point below 1.0 means the incoming cables, transformer and generator are carrying current that does no useful work.

The practical effects on an industrial site:

- Higher current for the same kW load, which pushes cable and switchgear closer to their rated capacity and increases resistive losses (heat) in the distribution system.
- A generator or transformer that reaches its kVA limit before it reaches its kW limit, so usable output is capped below the nameplate rating.
- On some tariff structures the utility bills a power factor penalty once it falls below a threshold; where that applies to your account, the tariff schedule states the threshold and the penalty formula.

Power factor correction addresses the first two directly. The third depends on your specific tariff class and should be checked against your bill, not assumed.

## Correction Options: Fixed Bank, Automatic Panel or Detuned Bank

There are three broad ways to add capacitive reactive power to a distribution board, and the right one depends on how much the load varies through the day and how much harmonic distortion is already on the busbar.

For the plain relationship between kW, kVA and power factor before comparing the options below, see our explainer on [what power factor is](/blog/power-factor-explained/).

A fixed capacitor bank switches in a set amount of kVAr and stays connected while the equipment it is correcting runs. It suits a single large, steady load such as a fixed-speed compressor or a bank of similar motors that run together for long stretches. It is the simplest and cheapest option, but if the load drops and the capacitors stay connected, the power factor can swing from lagging to leading, which on a generator supply is the condition covered below.

An automatic power factor correction (APFC) panel, also called an automatic power factor correction panel or APFC panel, uses a controller and current transformer to measure the actual power factor in real time and switch capacitor steps in and out through contactors or thyristor switches to hold the target power factor as load varies. This is the standard choice for a factory or facility with a mixed, fluctuating load: intermittent motor starts, shift changes, seasonal HVAC swings. The controller needs correct CT polarity and a target set point (commonly around 0.95 to 0.98 lagging, never a leading target on a generator-fed board) or it will hunt between steps.

A detuned capacitor bank adds a reactor in series with each capacitor step. The reactor does nothing at the fundamental 50 Hz frequency but presents rising impedance as frequency rises, which stops the bank from becoming a low-impedance path for harmonic currents. Where the site already has variable frequency drives, UPS systems, rectifiers or arc welding, a plain (non-detuned) bank risks a phenomenon covered in the next section, and a detuned design is the safer specification.

## Detuning: Why Harmonics Change the Design

A capacitor and the site's supply inductance form a resonant LC circuit. If that resonant frequency lands close to a harmonic already present on the system, commonly the 5th (250 Hz) or 7th (350 Hz) on a 50 Hz network, the bank amplifies that harmonic instead of correcting power factor. The result is capacitor fuse operation, overheating capacitors, nuisance tripping of protective devices and, in bad cases, damage to other equipment sharing the busbar.

A detuned reactor shifts the bank's resonant point below the lowest significant harmonic present, so the filter behaves as a capacitor at 50 Hz and as a harmonic-blocking inductor above it. Manufacturer datasheets describe this in terms of a detuning factor, expressed as a percentage or as a tuning order (for example, values in the region of 5.67% or 7% correspond to different target orders), and the correct value depends on the harmonic spectrum actually measured on site, not a default. Where a plant has significant non-linear load, a power quality survey that measures the harmonic spectrum before specifying the bank is worth the time it takes; guessing the detuning factor is how sites end up replacing capacitors repeatedly.

## The Generator Risk: Leading Power Factor and AVR Instability

Most power factor guidance is written for a grid connection, where the utility's fault level is effectively infinite and absorbs whatever reactive power a slightly over-corrected bank produces. An industrial or diesel generator does not have that headroom.

When capacitors over-correct a generator's load, the current can shift from lagging to leading. A synchronous generator's automatic voltage regulator is designed to respond to a lagging, inductive load; under a leading power factor the machine is effectively absorbing reactive power rather than supplying it, and the AVR's normal control response can become unstable. Symptoms include voltage hunting (the output oscillating rhythmically instead of holding steady), sustained overvoltage, or the AVR driving toward its excitation limits. Left running like this, the generator can trip on overvoltage or undervoltage protection, and prolonged operation outside its excitation limits stresses the exciter and rotating diodes. Our posts on [generator low output causes](/blog/generator-low-output-causes/) and [AVR faults](/blog/generator-avr-faults/) cover what a struggling voltage regulator looks like from the output side, whatever the underlying cause.

The practical rule for a generator-fed board: never target unity or leading power factor with a fixed or automatic bank. Set the APFC controller's target comfortably inside the lagging region, commonly quoted around 0.95 lagging, and disconnect or reduce capacitor steps automatically when load drops rather than leaving a fixed block of kVAr connected to a lightly loaded generator. If the site runs partly on grid and partly on generator, the correction scheme needs to account for both conditions, because a bank sized correctly for the grid connection can easily over-correct a smaller generator running the same board on an outage.

## Comparing the Three Options

| Type | How it corrects | Best suited to | Watch for |
|---|---|---|---|
| Fixed bank | Fixed kVAr connected continuously | One large, steady load; simple boards | Leading power factor when load drops, especially on generator supply |
| Automatic (APFC) panel | Controller switches kVAr steps to track load | Mixed, fluctuating industrial load | CT polarity, contactor wear from frequent switching, correct target set point |
| Detuned bank | APFC or fixed bank with series reactors | Sites with VFDs, UPS, rectifiers or other harmonic-generating load | Detuning factor must match the actual harmonic spectrum, not a default value |

## Sizing a Bank: Work From the Actual Load

Sizing starts from the kW load and the existing power factor, not from a target kVAr figure taken off a brochure. The general relationship is:

Required kVAr = kW x (tan(cos-1 existing PF) minus tan(cos-1 target PF))

Take a hypothetical facility with a steady 400 kW load at 0.72 lagging power factor, targeting 0.95 lagging. Applying the formula above (tan of the angle at 0.72 is roughly 0.964, tan of the angle at 0.95 is roughly 0.329) gives a requirement in the region of 254 kVAr. That figure is illustrative of the method, not a spare-part or purchase recommendation; an actual specification needs a load survey across a representative period, because a single instantaneous reading understates or overstates the swing an automatic panel has to track. Our [power plant audits and diagnostics](/power-plant-audit-nigeria/) service covers this kind of load and harmonic survey before a bank is specified.

## Maintenance of Capacitor Banks

Capacitors degrade with heat, harmonic loading and age, and a bank that was correctly sized on day one can drift out of tolerance well before it fails outright. A maintenance routine for an industrial APFC or detuned bank typically covers:

- Visual inspection of capacitor cans for bulging, leakage or discolouration, and of contactors for pitting from switching.
- Checking capacitance of each step against nameplate value; a capacitor commonly reads low once it has lost a meaningful fraction of its rated capacitance, which is a sign of internal element failure, not something to leave until it fails completely.
- Torque-checking busbar and cable connections, since a loose joint under capacitor switching current runs hot.
- Reviewing the controller's logged power factor and step-switching frequency for signs of hunting or a target set point that no longer matches the load.
- Confirming discharge resistors or devices bring residual voltage down to a safe level within the time stated on the panel before any cover is opened.

Capacitor banks store energy and can retain a dangerous residual charge after the supply is switched off, and the panels sit inside boards carrying other live circuits. Testing, discharging or internal inspection of a capacitor bank needs a qualified electrical technician working to lockout/tagout procedure under a permit to work, not a general handyman fix. This is not a task to attempt from a written guide.

## Where Correction Fits in a Wider Power Review

Power factor correction is one line item in a broader power quality and efficiency picture that usually also covers harmonic distortion, unbalanced loading, generator sizing against actual demand and the condition of the switchgear feeding the capacitor bank. Fixing power factor in isolation, without checking what is generating the harmonics in the first place, is how a site ends up replacing a plain bank with a detuned one within a year of installing it. A site-wide [power plant audit and diagnostics](/power-plant-audit-nigeria/) review puts the capacitor bank decision in that context, measuring the actual load and harmonic profile before recommending fixed, automatic or detuned correction. Nuisance tripping from an under-specified or badly detuned bank has a real cost too; see our post on [plant downtime cost per hour](/blog/plant-downtime-cost-per-hour/) for how to put a figure on that risk. If your plant is weighing a capacitor bank against a wider power review, [request a technical proposal](/#contact) and we will scope the survey against your board and your load.

## Frequently Asked Questions

### What is a good power factor target for an industrial site?

Most APFC controllers are set to hold between 0.93 and 0.98 lagging, comfortably inside the lagging region so the board never drifts into a leading condition. The exact target should reflect your tariff structure where a penalty threshold applies, and on a generator-fed board it should never be set to unity or leading.

### Do I need a detuned capacitor bank or will a standard one do?

If the board already carries variable frequency drives, UPS systems, rectifiers or significant welding load, a standard bank risks resonating with the harmonics those loads produce. A harmonic spectrum measurement on the actual board is the reliable way to decide, rather than assuming either way.

### Can power factor correction damage my generator?

Correction itself does not damage a generator, but over-correcting a generator-fed board into a leading power factor can destabilise the AVR's voltage control and push the machine toward its excitation limits. Sizing the bank, or setting the APFC target, against the generator's actual running load rather than the grid connection's load avoids this.

### How often should a capacitor bank be inspected?

A practical routine checks contactor condition and controller logs monthly and measures each step's actual capacitance against nameplate value at least twice a year, more often in hot, dusty conditions or where switching is frequent. A capacitor reading meaningfully below its rated capacitance should be treated as failing, not monitored indefinitely.

### Does power factor correction reduce fuel consumption on a generator?

Correcting power factor reduces the reactive current the generator has to supply for the same real (kW) load, which frees up kVA headroom rather than directly cutting fuel burn, since fuel consumption tracks real power delivered. Where a generator was previously current-limited by a poor power factor before reaching its kW rating, correction can let it deliver more usable kW from the same set.
