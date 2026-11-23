---
meta_title: "Generator Protection Relay: ANSI Codes and Settings"
meta_description: "What each generator protection relay function does, from 27/59 and 32 to 87G and 40, which ones a genset controller covers, and why settings drift."
primary_keyword: "generator protection relay"
secondary_keywords: "generator protection functions, ansi codes generator protection, generator protection scheme, reverse power relay"
---

# Generator Protection Relay Functions and ANSI Codes: What Each One Does and Where Settings Go Wrong

Open the protection page on almost any generator panel and you'll find a list of numbers: 27, 59, 81, 32, 40, 46, 50, 51, 87G. Operators know the ones that trip the set often enough. Few people on site can say what the rest are watching for, or when anyone last checked the thresholds against the plant as it runs today.

That's the real issue with a generator protection relay. The device itself is rarely the problem. The settings inside it were calculated once, for a machine and a network that no longer match what's on site. This article walks through the standard functions by their ANSI device numbers, shows how a small diesel set differs from a large turbo-generator, and explains how settings drift and how you catch it.

## What a generator protection scheme is actually protecting

A generator protection scheme has three jobs. It protects the machine from faults inside it (stator and rotor damage), from abnormal conditions the outside world forces on it (unbalanced load, low frequency, motoring), and it protects the rest of the plant from a failing machine. Those are different risks, and they need different measurements.

The functions are numbered by a standard, ANSI/IEEE C37.2, which assigns a device number to each protective function. Manufacturers add suffixes (the "G" in 87G means generator, the "N" in 51N means neutral or earth current), but the base numbers are the same on every relay from every maker. That's the useful part. Once you know the numbers, a Deep Sea panel, a Woodward multifunction relay and a turbine manufacturer's protection cabinet all read the same way.

## The functions in plain terms

Voltage first. Device 27 is undervoltage and 59 is overvoltage. A generator that loses excitation control (a failing AVR is the usual cause, see [AVR faults](/blog/generator-avr-faults/)) can drift either way, and both damage connected equipment. 59 also guards the machine's insulation.

Frequency next. 81U trips on under-frequency and 81O on over-frequency. Under-frequency on a loaded set generally means the engine or turbine can't hold speed, and on a grid-connected machine it's an early sign of a network in trouble. Over-frequency means speed control has gone wrong.

Device 32, the reverse power relay, detects the generator motoring: drawing real power from the bus instead of delivering it. On a diesel set that means the engine has lost fuel or power and the alternator is turning it. The danger is mechanical, not electrical. A reciprocating engine being driven can suffer damage and fire risk, and a steam turbine motoring loses steam flow through the blades, which overheats the last stages. A gas turbine being motored is stressing a compressor that was never meant to be driven backwards.

Device 40 is loss of field. If excitation disappears while the set is paralleled, the machine runs as an induction generator and pulls large reactive current from the bus, while rotor surfaces heat from induced currents. It matters much more on big machines, but any set running in parallel with others or the grid can suffer it.

Device 46 is negative sequence (unbalance) protection. Unbalanced stator currents produce a field rotating backwards relative to the rotor, which heats the rotor surface. The machine's withstand is expressed as I2 squared times time, a constant the manufacturer supplies. Small sets rarely get a dedicated 46, though phase unbalance still shows up as a different kind of problem on the load side.

Devices 50 and 51 are instantaneous and time-delayed overcurrent. 51V, voltage-restrained or voltage-controlled overcurrent, solves a specific problem: a generator's fault current collapses as its terminal voltage dips, and can fall below the normal load current setting before the relay times out. By lowering the pickup as voltage falls, 51V stays alert to remote faults a plain 51 would miss.

Device 87G is generator differential. It compares current into each winding with current out of it, and trips instantly for an internal phase-to-phase or phase-to-earth fault, without waiting for a time delay. It's the fastest and most selective protection a generator has, and its job is to limit damage once insulation has already failed.

Earth faults split in two. 51N sees earth current through the neutral earthing, and works well when the machine is earthed through a resistor or solidly earthed. On high-impedance earthed machines, where the neutral connects through a transformer and resistor, fault current is limited to a few amperes and the protection looks at neutral voltage instead (64G, stator earth fault). How the neutral is earthed decides which of those you need, and [generator earthing](/blog/generator-earthing-industrial/) covers that choice in detail.

Device 24 is overfluxing (volts per hertz). Voltage rising or frequency falling pushes the core into saturation and overheats it. It matters mostly during run-up, run-down and excitation faults on larger machines and on any unit with a step-up transformer. Device 49 is thermal overload, modelling winding temperature from current history or reading RTDs. Device 25, synch check, supervises closing the breaker so a set only parallels when voltage, frequency and phase angle are within a tight window. [Generator synchronization](/blog/generator-synchronization/) explains why a bad close is so destructive.

## ANSI codes for generator protection: small diesel set vs large turbo-generator

The table below shows how those functions typically get applied. Treat it as a typical pattern, not a rule. The exact set depends on machine size, voltage, earthing, how the set connects to the network and what the manufacturer's warranty requires.

| ANSI code | What it detects | Small diesel set (say, up to a few MVA, LV) | Large turbo-generator (MV, step-up transformer) |
|---|---|---|---|
| 27 / 59 | Under / overvoltage | Built into the genset controller, tripping or alarming | Separate relay, often two stages each |
| 81U / 81O | Under / over frequency | Built in, usually the same unit as 27/59 | Staged to match turbine blade resonance limits |
| 32 | Reverse power (motoring) | Common where sets run in parallel, small percentage pickup | Always fitted, set low and timed carefully, often two elements |
| 40 | Loss of field | Rare on small sets | Standard, mho or impedance elements |
| 46 | Negative sequence | Usually absent or basic unbalance alarm | Standard, matched to the machine's I2 squared t curve |
| 50 / 51 | Short-circuit and overload current | Built in, a basic inverse or definite time curve | Backup behind differential, coordinated with grid and transformer |
| 51V | Overcurrent restrained by voltage | Seen on parallel sets with weak fault contribution | Standard backup |
| 87G | Phase differential | Mostly not fitted below a few MVA | Standard on virtually all larger units |
| 64 / 51N | Stator earth fault | Neutral overcurrent if resistor earthed | 64G (95 percent and often 100 percent with third harmonic) on high-impedance earthing |
| 24 | Overfluxing | Not normally fitted | Fitted, especially with a unit transformer |
| 49 | Thermal overload | Winding RTD alarm or trip | Thermal model plus RTDs |
| 25 | Synch check | Built into the controller or the sync module | Dedicated, often with check synch redundancy |

The trend is plain. The bigger and more valuable the machine, the more of the protection is its own dedicated relay with its own CT inputs, and the more of it overlaps. The small set depends on its controller doing several jobs at once.

## What sits in the genset controller and what needs a separate relay

Modern genset controllers do more than most people assume. A typical unit covers voltage and frequency (27/59/81), overcurrent (50/51), reverse power (32) on paralleling versions, and often synch check (25) through its load-sharing module. For a standby diesel set serving a single site, that's usually adequate. For the alarm and trip list on these controllers see [Deep Sea controller alarms](/blog/deep-sea-controller-alarms/).

A separate multifunction relay becomes worth it when one or more of these is true: the set is above a few MVA, it runs in parallel with the grid, it's medium voltage, it feeds a step-up transformer, or the loss of the unit would stop the plant. Differential (87G) is the clearest case. It needs current transformers on both sides of the winding, and a controller that only reads output current can't do it.

One rule covers most sites: if the machine is on the main process for a plant that can't stop, don't ask a controller to be the whole protection scheme. A controller is built to run an engine and share load. A relay is built to see a fault in a few cycles and open a breaker. Using one for the other's job works until the day it doesn't.

Separate relays aren't automatically better. A relay with 12 functions switched on and default settings protects nothing. Fewer functions with calculated, tested settings beat a full feature list left at factory values.

## Why settings drift from reality

Settings are calculated for a particular machine, a particular load and a particular network. All three move.

Take a hypothetical plant that sized its overcurrent settings when the generator fed a small building load. Two years later, the plant adds a few large motors and a longer cable run. The thermal and short-circuit conditions have changed, but the relay still carries the original curve. Either it trips on a motor start it should ride through, or it fails to see a fault at the end of the new feeder, because the fault current there is lower than the pickup.

The same happens on the network side. When a plant that used to run only on its own generator starts paralleling with the grid, or when a DISCO supply changes its fault level, the reverse power and frequency settings that suited island operation may not suit parallel running. Transformer replacements, a new neutral earthing resistor, a changed CT ratio during an upgrade, and a controller swapped like for like with default settings all do the same damage quietly. Check the current requirements for grid-connected operation with the regulator and the DISCO, because those rules change.

Three other causes come up repeatedly. Someone widens a trip threshold to stop nuisance trips and never records it. A CT ratio entered in the relay doesn't match the one actually installed. And a trip function gets switched to alarm only during commissioning and never put back. Each is invisible until the day the protection is needed.

## Setting reviews and secondary injection testing

A setting review compares what's in the relay with what the plant needs today. It starts with current data: generator nameplate and reactance values, CT and VT ratios, the earthing arrangement, transformer details, upstream protection settings and the present load profile. From that, someone recalculates the pickups and delays and checks them against what's loaded. Where they differ, the engineer finds out why, because sometimes the odd setting exists for a good reason nobody wrote down.

Secondary injection testing then proves the relay does what the setting file says. A test set injects voltage and current into the relay's secondary inputs and checks pickup values, timing and the output contacts that trip the breaker and shutdown solenoid. That also proves the trip path is intact, which a setting printout can't.

It doesn't prove the primary side. CT polarity, ratio and wiring errors need primary injection or other checks. Backward polarity on a differential or reverse power CT, for instance, passes a secondary test while the real thing behaves wrongly. [Megger insulation testing](/blog/megger-test-insulation-resistance/) of the windings is a different job, but it belongs in the same outage window.

Any hands-on testing on a live installation needs the set isolated, locked out and tagged, with a permit to work in place. That includes the trip circuits: disconnect or block them from the breaker and the fuel solenoid deliberately, so a test signal can't operate plant that's still running. Forgotten blocking links after a test are a classic way to end up with a relay that "tests fine" and trips nothing.

A sensible interval depends on the relay type, the criticality of the machine and what the manufacturer or the plant's own procedures state. Review settings again whenever the electrical network changes, not on the calendar alone.

## Grid problems and generator protection

Frequency and voltage functions matter most when the network misbehaves. A weak grid collapsing around a plant can leave a paralleled generator trying to carry loads it was never sized for, or tripping on frequency just when the plant needs it. [Grid collapse and plant protection](/blog/grid-collapse-plant-protection/) covers how those events develop and what a plant should expect from its protection during them. If the plant's islanding or load-shedding scheme and the generator relays aren't coordinated, the generator may trip before the shedding has done its work, or the reverse.

If you're unsure whether the protection on your generators still matches the plant, [request a technical proposal](/#contact) for a protection settings review and relay testing.

## Frequently Asked Questions

### What is a generator protection relay?

It's a device that monitors a generator's voltage, current, frequency and other quantities and trips the breaker, or shuts the set down, when a measurement shows a fault or dangerous condition. Modern ones are digital multifunction relays that combine many ANSI functions, such as 27, 59, 81, 32, 40, 46, 51 and 87G, in one unit. Smaller sets often rely on the protection built into the genset controller instead.

### What does a reverse power relay do on a generator?

A reverse power relay (device 32) detects the generator drawing real power from the bus instead of supplying it, meaning the set is motoring. That happens when fuel, steam or gas is lost while the breaker remains closed. It trips the set off the bus so the prime mover isn't dragged around by the alternator, which can damage a diesel engine or overheat steam turbine blades.

### Does a diesel generator need differential protection?

Not always. Differential protection (87G) is standard on larger machines because it clears internal winding faults quickly, limiting damage. On small low voltage standby sets it's usually omitted and overcurrent and earth fault protection does the work. The decision depends on machine size, voltage, value and consequence of loss, so it should be made by an engineer who has the single line diagram in front of them.

### How often should generator protection settings be reviewed?

There's no single interval that fits every plant. Review settings after any change to the load, the network connection, the earthing, the CT ratios or the relay itself, and as part of the periodic maintenance programme. Secondary injection testing at planned outages proves the relay still operates as set, and a documented settings file makes later reviews far faster.

### Can a genset controller replace a separate protection relay?

On a small standby set serving one site, the controller's built-in protection is often enough. On larger, medium voltage, grid-paralleled or process-critical machines, it isn't, because a controller can't provide functions like differential or loss of field and isn't built for fast fault clearance. The two do different jobs, and the more the plant depends on the machine, the stronger the case for a dedicated relay.
