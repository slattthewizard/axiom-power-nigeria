---
title: "Power Factor Explained: What It Means for Your Plant's Generators and Electricity Costs"
navTitle: "Power Factor Explained: What"
metaTitle: "Power Factor Explained for Nigerian Plant Managers"
metaDescription: "Power factor explained in plain terms: what causes lagging power factor, its effects on generators and cables, and how Nigerian plants measure and fix it."
primaryKeyword: "power factor"
secondaryKeywords: "what is power factor, power factor meaning, lagging power factor, low power factor effects"
publishedDate: "2026-10-10"
tag: "Generators"
subtitle: "A maintenance manager who has never had to think about power factor usually meets it for the first time when the generator starts hunting on voltage, a cable feeding a motor bank runs hotter than it..."
canonical: "https://axiompowerng.com/blog/power-factor-explained/"
faq:
  - question: "What is power factor in simple terms?"
    answer: "Power factor is the ratio of real power (kW), the power that does useful work, to apparent power (kVA), the total power your generator or transformer has to supply. A ratio of 1.0 means all supplied power is being used productively; anything lower means part of the current flowing is reactive current that magnetic components need but that does no work."
  - question: "What does a lagging power factor mean?"
    answer: "Lagging power factor means the current waveform lags behind the voltage waveform, which happens because inductive loads such as motors and transformers need magnetising current. It is the normal condition on almost every industrial site and is corrected, when it gets too low, with capacitor banks rather than by removing the motors causing it."
  - question: "Why do generators derate at a lower power factor?"
    answer: "A generator alternator is designed to deliver its full kVA rating at a specific power factor, usually 0.8 lagging. Below that power factor, the same alternator supplies the same total kVA but a smaller share of it converts to usable kW, so the plant effectively loses real power capacity without the generator itself failing or being undersized."
  - question: "Can power factor damage equipment?"
    answer: "Sustained low power factor does not damage equipment suddenly, but it increases current for a given amount of useful work, which raises heating in cables, motor windings and transformer coils over time and can shorten insulation life. A power factor that swings to leading, usually from an oversized capacitor bank, can also destabilise a generator's voltage regulation."
  - question: "How often should power factor be checked?"
    answer: "Power factor should be logged continuously through the genset controller or plant metering where available, and reviewed whenever load patterns change significantly, such as adding new motors or drives. A single spot reading is not reliable evidence either way, since power factor moves with what is running at the time it is taken."
---
A maintenance manager who has never had to think about power factor usually meets it for the first time when the generator starts hunting on voltage, a cable feeding a motor bank runs hotter than it should, or a DisCo bill shows a reactive power charge nobody can explain. Power factor is not an abstract utility metric. It is a measure of how efficiently the current your plant draws is actually doing useful work, and it directly affects how hard your generators, cables and transformers have to work to deliver the same output.

This article sets out what power factor is, why it drops, and what a low or lagging power factor does to plant equipment. It is written for the person running the plant, not the person designing it, so the maths is kept to what you need to read a nameplate, a meter reading, or a DisCo bill correctly.

## What Power Factor Actually Measures

Every AC load draws two kinds of power. Real power, measured in kW, is the power that does actual work: turning a shaft, producing heat, lighting a bulb. Apparent power, measured in kVA, is the total power your source (generator or transformer) has to supply to deliver that real power, once you account for the current needed to build and collapse magnetic fields in motors, transformers and ballasts.

Power factor is simply the ratio between the two:

Power factor = kW ÷ kVA

A power factor of 1.0 means every kVA the generator supplies converts into kW at the load. In practice, no industrial plant sits at 1.0, because motors, transformers and some lighting and drive loads are inductive: they need magnetising current that does no work but still has to flow through the alternator windings, the cables and the switchgear. That is why generator nameplates are rated in kVA at 0.8 lagging power factor as standard, not in kW. If your plant's power factor is below 0.8, the generator is not delivering its full rated kW even though it is fully loaded in kVA terms. The relationship between kVA and kW is covered in detail, with worked examples, on our kVA to kW conversion guide.

## Lagging and Leading Power Factor

The word "lagging" describes the normal condition in an industrial plant. Inductive loads, motors above all, cause the current waveform to lag behind the voltage waveform. The bigger the inductive load relative to real load, the further the current lags and the lower the power factor number.

Leading power factor is the opposite: current runs ahead of voltage, which happens when capacitive loads dominate, or when power factor correction capacitors are oversized for the load they are connected to. Leading power factor on a plant running its own generator is worth flagging early, because it interacts badly with the alternator's automatic voltage regulator and can cause voltage instability, covered further down.

## What Causes a Low Power Factor on an Industrial Site

Most low power factor problems in Nigerian plants trace back to a small set of causes:

- **Induction motors**, which are the single biggest source of lagging power factor on almost every factory, pumping station or workshop floor. A motor's own power factor is not fixed: it changes with load.
- **Lightly loaded motors.** A motor sized for a duty it rarely reaches, common where a plant has over-specified drives "to be safe", runs at a much worse power factor than the same motor near full load. Magnetising current stays roughly constant while useful current drops, so the ratio gets worse.
- **Old fluorescent lighting ballasts**, welding sets and some variable frequency drives, which add their own reactive or harmonic-distorted current.
- **Transformers running lightly loaded**, for the same reason as motors: the no-load magnetising current becomes a larger share of total current.
- **A plant with a lot of idle or standby equipment** still energised but not doing work, which adds reactive current with no real power to show for it.

None of these are faults in the individual sense. A motor running at 40 per cent of its rated load with a poor power factor is doing exactly what an induction motor does under those conditions. The fix is at the system level: right-sizing loads, running motors closer to their design duty, and correcting the reactive component with capacitors, which we cover in a separate article on power factor correction and capacitor banks.

## Effects of Low Power Factor on Generators

This is the part most plant managers actually feel first. A generator alternator is designed and rated around a specific power factor, almost always 0.8 lagging. Running the plant at a worse power factor than that has three practical effects:

1. **The generator cannot deliver its full kW rating.** A 500 kVA alternator at 0.8 pf gives you 400 kW. At 0.6 pf, the same alternator still caps out around 300 kW of real power even though it is working just as hard in kVA terms, so you effectively lose usable capacity you already paid for.
2. **The AVR works harder and can hunt.** Excess reactive current, especially a swing toward leading power factor from oversized or poorly switched capacitor banks, pushes the automatic voltage regulator outside its stable operating band. Voltage hunting, flickering lights and nuisance trips on sensitive equipment often trace back to this rather than to the AVR itself. Our article on generator low output causes goes through the fuller diagnostic order, of which power factor is one branch.
3. **The alternator runs hotter for the same real load**, because current, not power, is what heats the windings. A poor power factor means more current for the same kW delivered, which shortens insulation life over time and adds to the wear the maintenance programme has to manage.

None of this shows up as a single alarm. It shows up as a generator that seems undersized, an AVR that seems unreliable, or an alternator that runs warmer than its rating suggests it should, all of which are easier to diagnose once power factor is checked and ruled in or out.

## Effects on Cables, Switchgear and Transformers

The same principle: current, not real power, is what determines heating and voltage drop in a cable or a transformer winding. A cable sized correctly for a load at 0.85 power factor will run hotter, and drop more voltage along its length, if the actual operating power factor falls to 0.65, because more current is flowing to deliver the same kW. Over years this shows up as insulation ageing faster than expected and as voltage at the far end of a feeder being lower than calculations suggest it should be. Transformers see the same effect: apparent power (kVA) loading, not real power, is what determines how close a transformer sits to its thermal limit.

| Symptom on site | Likely power factor cause | What to check |
|---|---|---|
| Generator "underpowered" despite correct kVA sizing | Plant running below 0.8 pf, lagging | Measure pf at the genset switchboard under normal load |
| AVR hunting, voltage flicker | Leading pf from oversized or badly staged capacitor bank | Check capacitor bank staging against actual load, not rated load |
| Cables or motor terminals running hot | High reactive current for the real load carried | Compare measured current to the current implied by kW alone |
| DisCo or metering shows a reactive energy charge | Sustained low power factor on the incomer | Log pf over a full production cycle, not a single reading |
| Transformer loading looks high on kVA but low on kW | Lightly loaded motors or standby transformers on the same bus | Audit motor loading against nameplate rating |

## How to Measure Power Factor

Power factor is read directly off a power quality analyser or a modern digital meter fitted to the switchboard or the generator control panel; most genset controllers and many modern distribution panels display it continuously alongside voltage, current and frequency. A single snapshot reading is of limited use, because power factor swings through the day with what is switched on. What matters for diagnosis and for correction sizing is a logged reading over at least one full production cycle, capturing peak motor-starting periods and low-load periods such as night shift or shutdown standby. A power plant audit is the right point to capture this properly, alongside the other electrical parameters that affect generator loading and cable condition, rather than treating power factor as a one-off measurement.

If your plant's own metering does not show power factor, or the figure looks implausible, the safest step is a proper measurement campaign rather than guesswork from a nameplate calculation, since actual operating power factor almost always differs from the design assumption once real loads and their duty cycles are accounted for.

## Correcting a Low Power Factor

Correction is a separate subject from measurement, and it is easy to get wrong: an undersized capacitor bank barely moves the needle, an oversized one pushes the plant into leading power factor and destabilises the generator's AVR, and a bank installed without detuning on a site with variable frequency drives or other harmonic-generating loads can resonate and fail early. Our dedicated article on power factor correction and capacitor banks covers fixed versus automatic banks, detuning, and the specific risk a leading power factor poses when the plant is running on its own generator rather than the grid.

Before specifying any correction equipment, get an accurate picture of where your plant actually sits, request a technical proposal for a plant assessment, or start with our power plant audits and diagnostics service, which measures power factor alongside load profile, harmonics and generator loading in one exercise rather than treating each symptom separately.

## Frequently Asked Questions

### What is power factor in simple terms?

Power factor is the ratio of real power (kW), the power that does useful work, to apparent power (kVA), the total power your generator or transformer has to supply. A ratio of 1.0 means all supplied power is being used productively; anything lower means part of the current flowing is reactive current that magnetic components need but that does no work.

### What does a lagging power factor mean?

Lagging power factor means the current waveform lags behind the voltage waveform, which happens because inductive loads such as motors and transformers need magnetising current. It is the normal condition on almost every industrial site and is corrected, when it gets too low, with capacitor banks rather than by removing the motors causing it.

### Why do generators derate at a lower power factor?

A generator alternator is designed to deliver its full kVA rating at a specific power factor, usually 0.8 lagging. Below that power factor, the same alternator supplies the same total kVA but a smaller share of it converts to usable kW, so the plant effectively loses real power capacity without the generator itself failing or being undersized.

### Can power factor damage equipment?

Sustained low power factor does not damage equipment suddenly, but it increases current for a given amount of useful work, which raises heating in cables, motor windings and transformer coils over time and can shorten insulation life. A power factor that swings to leading, usually from an oversized capacitor bank, can also destabilise a generator's voltage regulation.

### How often should power factor be checked?

Power factor should be logged continuously through the genset controller or plant metering where available, and reviewed whenever load patterns change significantly, such as adding new motors or drives. A single spot reading is not reliable evidence either way, since power factor moves with what is running at the time it is taken.
