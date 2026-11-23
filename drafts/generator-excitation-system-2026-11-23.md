---
meta_title: "Generator Excitation System: How It Works and What Fails"
meta_description: "How a generator excitation system works: brushless exciter, PMG, static excitation, the AVR, common faults, loss of excitation and safe test methods."
primary_keyword: "generator excitation system"
secondary_keywords: "brushless excitation, generator excitation explained, static excitation, loss of excitation"
---

# Generator Excitation System Explained: Brushless, PMG and Static Excitation, and the Faults That Stop Them

A synchronous generator makes no voltage until its rotor carries direct current. The engine or turbine supplies the mechanical power, but the excitation system supplies the magnetic field, and that field decides your terminal voltage and, once you're in parallel, how much reactive power the machine gives or takes. When a set spins at 1,500 rpm with no output, or the voltage sags every time a big motor starts, the excitation system is usually where the problem lives.

## What the excitation system actually does

The rotor of a synchronous generator is an electromagnet. Push DC through its winding and, as the rotor turns, the field cuts the stator windings and induces the three-phase voltage. More field current means more terminal voltage.

Two jobs follow from that. First, set the no-load voltage at the right value, 415 V on most Nigerian industrial sets. Second, hold that voltage as load changes, because a loaded stator drops voltage through its own reactance and armature reaction. The excitation system raises the field current as the load and its lagging power factor increase, and backs it off when the load falls away.

When the generator is paralleled with the grid or with other sets, the bus largely pins the voltage. Changing the field current then changes the reactive power (kVAr) the machine exports or imports, not the voltage.

## Brushless excitation: the standard on diesel sets

Nearly every diesel generator from a few kVA up to several MVA uses brushless excitation. There are no slip rings and no carbon brushes. Instead there are two machines on one shaft.

The main exciter is a small alternator turned inside out. Its field winding is stationary, in the stator, and its three-phase armature is on the rotor. The AVR feeds a small DC current into the stationary exciter field. The rotating exciter armature produces AC, which goes straight to a rotating rectifier, a ring or wheel of diodes bolted to the shaft. The rectified output feeds the main generator field winding, also on the rotor. Everything from the exciter armature to the main field turns together, so no brushes are needed to carry the current across.

The advantage is plain: nothing to wear and no brush dust in the alternator. The cost is that you can't measure the main field current while it runs, and anything that breaks on the rotating side is out of reach until the set is stopped and isolated.

Most rotating rectifiers also carry a surge suppressor, a varistor or resistor-capacitor network across the DC side, to protect the diodes from voltage spikes. These parts fail more often than people expect.

## Self-excited, shunt and PMG-supported excitation

How the AVR gets its power is the real dividing line between a cheap alternator and a good one.

In a self-excited (shunt) system, the AVR takes its supply from the generator's own output terminals. It's simple and cheap, and for steady loads it works. The weakness is the loop: if the terminal voltage collapses, the AVR loses its own supply right when it needs it most.

A permanent magnet generator, or PMG, is a small pilot alternator on the shaft with permanent magnets on the rotor. It produces its own voltage whenever the shaft turns, independent of the main stator. The AVR runs from that supply. So when a large motor starts and drags the terminals down, or a downstream short pulls the voltage toward zero, the AVR still has full power and can drive the exciter hard. That gives a PMG set its short-circuit support, typically around three times rated current for a few seconds on machines built for it, so protection can clear a fault selectively. Honestly, if you start big motors across the line, the PMG option is worth specifying.

| Arrangement | AVR supply | Strength | Weakness |
| --- | --- | --- | --- |
| Self-excited (shunt) | Generator terminals | Simple, low cost | Voltage dips can starve the AVR; weak fault current |
| PMG-supported | Shaft-mounted permanent magnet pilot | Rides through motor starts and faults | Extra machine to maintain |
| Static (slip ring) | Terminals via excitation transformer | Fast response, full control | Brushes, slip rings, bigger cabinet |

## Static excitation on large turbo-generators

On large turbo-generators and some bigger gas and steam units, the field power is taken from the generator terminals (or the station auxiliary supply) through an excitation transformer and a thyristor bridge. The controlled DC output goes to the rotor through carbon brushes running on slip rings.

Static excitation responds very quickly because there's no exciter machine in the loop, which helps stability on a big unit. The price is brushgear that needs routine inspection: brush length, spring pressure and ring surface condition.

## The AVR: what it senses and what it does

The automatic voltage regulator compares the generator voltage against a setpoint and adjusts the exciter field current to hold it. It senses voltage on two or three phases through sensing leads, and it carries a voltage adjustment, stability trimmers (the gain and damping that stop the voltage hunting) and an under-frequency roll-off.

The roll-off lowers the voltage setpoint when engine speed sags under a heavy load step, which cuts the kW the alternator demands and helps the engine recover. We cover AVR symptoms in [generator AVR faults](/blog/generator-avr-faults/), so here's just the point that wastes the most time: the AVR does what its sensing leads tell it. A loose or corroded sensing connection can read low, and the AVR will respond by driving the exciter to maximum. The generator then shows high voltage and the AVR looks guilty when it's doing exactly what it was told.

## Common excitation faults and how they show up

The pattern of the symptom usually points to the part.

A failed rotating diode is the classic. One diode shorting or opening unbalances the exciter armature. The set may still make voltage, but the exciter runs hot and the voltage is unstable under load. A shorted diode can overheat the exciter armature. A failed surge suppressor behaves similarly, sometimes with a burnt smell or tracking on the rectifier assembly.

Exciter winding faults are less common. An open or shorted exciter field gives little response to the AVR, which then hits its limit. The rotating armature can develop turn faults from heat and vibration, shown by unbalanced phase resistance.

Loss of residual magnetism is the "set runs, no voltage" fault. A shunt-excited machine needs a small remanent flux in the rotor iron to build up. It can be lost after long storage or a severe fault. With no residual flux there's nothing for the AVR to amplify and the voltage never builds. The fix is field flashing: a brief supply from a battery, applied to the exciter field with correct polarity, to restore the flux. Follow the manufacturer's procedure for voltage and duration, because wrong polarity can wipe out what little remains and a wrong connection can damage the AVR.

AVR sensing and supply faults round out the list. If output is low, work through the basics before you condemn the alternator. Our guide to [low generator output causes](/blog/generator-low-output-causes/) gives a sensible order of checks.

## Loss of excitation and what happens in parallel

If a generator running in parallel loses its field, the consequences are more serious than a voltage problem. Without field current, the machine can no longer hold synchronism through its field. It runs slightly above synchronous speed as an induction generator and draws large reactive power from the grid or the other sets to magnetise itself. The stator is overloaded by that reactive current, and the rotor heats because slip-frequency currents flow in the rotor body and damper windings, which weren't designed to carry them for long.

On a small bus with two or three sets, one machine losing field can pull the others toward their limits and bring the bus down.

Loss-of-excitation protection, usually relay code 40, detects the signature: the machine impedance moving into the reactive-importing region on the R-X plane. The relay trips the generator breaker and, depending on the scheme, the prime mover. Settings come from a protection study, not a guess, and the protection should be tested. Our guide to [generator synchronization](/blog/generator-synchronization/) covers the other half of safe paralleling.

## Testing the excitation system safely

Every one of these checks starts with the set stopped, the start system disabled, the generator breaker open and locked off, and a permit to work in place under your site's lockout-tagout procedure. A residual field and a turning shaft can still generate voltage, so isolation isn't optional.

With the set isolated, a competent technician can check the following.

Diode checks: with the rectifier accessible and the diodes disconnected from the winding if the manufacturer's procedure calls for it, use a multimeter on diode range. A healthy silicon diode reads a forward drop of roughly 0.3 to 0.7 V and is open in reverse. A reading near zero in both directions is shorted, and open in both directions is failed. Inspect the surge suppressor for discolouration or cracking.

Winding resistance: measure the exciter field, the exciter armature phases (closely balanced) and the main rotor field with a low-resistance ohmmeter. Absolute numbers vary by frame size, so compare against the last record and watch phase balance.

Insulation resistance: this is where careless testing destroys parts. Before you megger the rotor circuit, short out or lift the rotating diodes and the surge suppressor as the manufacturer instructs, because the test voltage can wreck semiconductors. Disconnect the AVR leads too. Then follow the method in our guide to the [megger test for insulation resistance](/blog/megger-test-insulation-resistance/), record the readings and discharge the winding afterwards.

Keep a baseline of winding resistance and insulation readings while the set is healthy. It turns a vague "something is wrong" into a clear comparison later.

If you'd like our engineers to look at a set with an unexplained voltage problem, or to check protection on paralleling sets, you can [request a technical proposal](/#contact) or book a plant assessment.

## Frequently Asked Questions

### What is a generator excitation system?

It's the equipment that supplies direct current to the rotor field of a synchronous generator so it can produce voltage, and controls terminal voltage and, in parallel, reactive power. Diesel sets usually use a brushless exciter with an AVR.

### Why does a generator run but produce no voltage?

The most common cause on a shunt-excited set is lost residual magnetism, so the voltage never builds up. Other causes are a failed AVR, a broken sensing or supply connection, an open exciter field or a failed diode. Isolate the set properly before you test or flash the field.

### What is the difference between PMG and shunt excitation?

A shunt-excited AVR takes its power from the generator output, so a deep voltage dip can starve it. A PMG is a small permanent magnet alternator on the shaft that powers the AVR independently of the main output. That's why PMG-supported sets handle large motor starts and short circuits better.

### What happens if a generator loses excitation while in parallel?

It stops holding synchronism through its field, runs as an induction generator and pulls heavy reactive current from the bus. That overloads the stator, heats the rotor and can destabilise the other sets. Loss-of-excitation protection exists to trip the machine quickly, and it should be set from a proper protection study.

### Can I megger the rotor of a brushless generator?

Yes, but not with the rotating diodes and surge suppressor in circuit, because the test voltage can destroy them. Isolate the set under a permit to work, short or lift the semiconductors as the manufacturer directs and disconnect the AVR before testing.
