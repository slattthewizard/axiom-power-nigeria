---
meta_title: "Star Delta Starter: How It Works and When to Skip It"
meta_description: "How a star delta starter cuts motor starting current and torque, why the transition trips faults, and when a soft starter suits a Nigerian plant better."
primary_keyword: "star delta starter"
secondary_keywords: "star delta starter working, soft starter, dol starter, motor starting methods"
---

# Star Delta Starter: How It Works, Where It Falls Short, and When to Move On

A motor that trips the incomer breaker every time it starts, or drags the generator's voltage down for a second before it recovers, usually has one problem in common: it is being started direct on line and the supply cannot absorb the inrush. A star delta starter is the classic fix for that, and it still runs a large share of the induction motors on Nigerian factory floors, pump houses and compressor rooms. It is cheap, it is well understood by most panel technicians, and for a fixed load with a light starting torque requirement it does the job. It is not, however, the only option, and on a site running off generators rather than a stable grid, the choice of starting method affects more than the motor.

This article covers how a star delta starter actually works, what current and torque reduction to expect, the transition fault that catches out a lot of installations, and where a soft starter or variable frequency drive earns its higher price. It also covers what motor starting does to a genset supplying the load, since that is the constraint that decides the method on many Nigerian sites more than the motor itself does.

## How a Star Delta Starter Works

A star delta starter uses three contactors and a timer to change the way a motor's stator windings are connected during starting. On start, the line contactor and the star contactor close together, connecting the three windings in a star configuration. Each winding then sees only the phase voltage (line voltage divided by root three) rather than the full line voltage it would see connected in delta. After a set time delay, usually somewhere between five and fifteen seconds depending on how long the motor takes to reach speed, the star contactor opens and the delta contactor closes, reconnecting the same windings across the full line voltage for normal running.

The controller side of this is simple: a timer relay, sometimes built into a dedicated star delta starter unit, sometimes wired discretely with a timer and a mechanical interlock between the star and delta contactors so the two can never close together. That interlock matters. A star and delta contactor closed at the same time puts a near dead short across two phases, which is one of the more expensive faults a panel technician can walk into.

## Current and Torque Reduction: The Numbers That Matter

The point of the star connection is that it cuts the voltage each winding sees to about 58 per cent of line voltage. Because starting current in an induction motor rises roughly with the square of applied voltage, the starting current drawn from the supply drops to close to one third of what direct on line starting would pull. Starting torque falls by the same proportion, since torque also varies with the square of voltage. A motor that would develop full-voltage starting torque of, say, 150 per cent of rated torque direct on line will develop roughly 50 per cent of rated torque in star.

That trade-off is the whole story with star-delta starting: a one-third reduction in current buys a one-third reduction in torque. For a load with low starting torque demand, a fan, a centrifugal pump running against a closed or partly closed valve, a lightly loaded compressor, that trade works well. For a load that needs strong starting torque, a loaded conveyor, a positive displacement compressor, a pump against a fully open valve, the motor can stall in star and never reach the speed needed to change over to delta. It sits there drawing locked rotor current in star, which the starter and cabling were never sized to hold indefinitely, and the thermal overload eventually (correctly) trips it.

## The Transition Problem

The step from star to delta is where most star-delta installations run into trouble, and it is worth understanding why. During the brief instant when the star contactor has opened but the delta contactor has not yet closed, the motor is coasting with no supply connected at all. Because the rotor still carries residual magnetic flux from the star connection, and that flux is now at the wrong phase relationship for a delta connection, closing the delta contactor produces a transient current spike, sometimes higher than the direct-on-line inrush the starter was installed to avoid, along with a sharp torque pulse.

Two things drive how bad that transient is: how long the open interval between star and delta lasts, and how much the motor has slowed during that interval. A timer set too generously, or a delta contactor that is slow to pull in, both stretch the open interval and make the transient worse. This is the practical reason a lot of star delta starter timers get retuned in the field rather than left at the factory default: the setting that suits one motor and load can produce a transition spike on a different motor and load, and the fix is usually a shorter, better-tuned delay rather than a longer one. A closed-transition starter, which briefly parallels star and delta through resistors before opening the star contactor, avoids the open interval and the current spike that goes with it, but it is a more expensive design and it is not common in retrofit panels.

## When a Soft Starter or VFD Does the Job Better

A soft starter uses thyristors to ramp voltage up smoothly from a set starting level to full voltage over an adjustable time, rather than switching between two fixed connections. That gives a controlled, stepless current profile with no transition transient, and it lets the ramp be tuned to the load rather than to two fixed voltage steps. For loads that need a gentler start than star-delta allows, or that are sensitive to the mechanical shock of a torque pulse (long conveyors, screw compressors, some pump and pipe combinations prone to hydraulic shock), a soft starter is usually the better fit at a modest cost premium over star-delta.

A variable frequency drive goes further: it varies both voltage and frequency, so it controls the starting current and also the motor's speed and torque continuously, during starting and during normal running. That makes a VFD the right choice where the process itself benefits from variable speed rather than a soft start alone, and our guide to [VFDs and how they affect generator loads](/blog/variable-frequency-drive-guide/) covers that trade-off and the harmonic distortion a VFD can put back onto a generator supply. Where a load runs at one fixed speed and the only requirement is a gentler start, the extra cost of a VFD over a soft starter usually is not justified.

| Starting method | Typical starting current (multiple of full load current) | Starting torque | Where it suits |
|---|---|---|---|
| Direct on line (DOL) | 6 to 8 x | Full (100%+) | Small motors, strong grid or generator, high torque needed |
| Star delta starter | 2 to 3 x | About one third of DOL torque | Low starting torque loads, cost-sensitive retrofits |
| Soft starter | 2 to 4 x, adjustable | Adjustable, smoother ramp | Torque-sensitive loads, no open transition wanted |
| Variable frequency drive | 1 to 1.5 x, adjustable | Full control, load-matched | Variable speed process, tightest current control |

These multiples are typical figures used across motor and starter manufacturer datasheets; the nameplate and starter manual for the specific motor and starter combination govern the actual figures for that installation.

## What Motor Starting Does to a Generator

On a grid connection with high fault capacity, a motor's starting current is a small disturbance the network barely notices. On a generator, the same current draw is a much larger fraction of what the alternator can supply, and the effect shows up as a voltage dip the moment the motor is switched in. A generator's AVR responds to that dip, but it takes a moment to react, and during that moment the voltage sag can be steep enough to drop out contactors, dim lighting circuits, or upset sensitive control electronics elsewhere on the same bus.

This is exactly why the choice of starting method matters more on a genset-supplied site than on a grid-supplied one. Cutting starting current from six or seven times full load current down to two or three times, which is what a star delta starter or soft starter does, brings the step load within what a correctly sized generator can accept without an unacceptable voltage dip. Our [generator sizing guide](/blog/generator-sizing-guide/) covers how to work out the step load a generator needs to accept, including the rule of thumb manufacturers publish for maximum single-step load as a percentage of the set's rating, and why that step load capability, alongside the running kVA, is what should drive the sizing conversation for a site with large motors. Where several motors start close together, or where one large motor is unavoidable, staggering starts and confirming the starter's actual current draw against the generator's step load rating is worth doing before the panel is commissioned, not after it has already caused nuisance trips.

If the current setup keeps tripping the generator's protection or the site's own breaker every time a motor starts, that is worth having assessed rather than solved by retiming a timer relay: repeated nuisance trips add up to real [downtime cost](/blog/plant-downtime-cost-per-hour/) over a year even when each individual trip is short. [Book a plant assessment](/#contact) with our engineers, or read more about the [rotating equipment services](/rotating-equipment-services-nigeria/) we cover, including motor and starter fault diagnosis on pumps, fans and compressors.

## Safety Note

Star delta starters, soft starters and VFDs all sit on live three-phase circuits carrying enough current to injure or kill, and the star-delta interlock fault described above is not a rare event in poorly maintained panels. Any work inside the starter cabinet, including retiming a transition delay, replacing a contactor, or diagnosing a nuisance trip, needs isolation, lockout and tagout, and a permit to work carried out by qualified personnel. This is not a job for trial and error with the cabinet live.

## Frequently Asked Questions

### What is the difference between a star delta starter and a soft starter?

A star delta starter switches the motor between two fixed connections, star for starting and delta for running, which gives a fixed current and torque reduction of roughly a third. A soft starter instead ramps voltage up smoothly using thyristors, giving an adjustable, stepless start with no transition spike, usually at a higher unit cost.

### Why does a star-delta transition sometimes cause a current spike?

Between the star contactor opening and the delta contactor closing, the motor coasts briefly with no supply connected, and residual flux in the rotor is at the wrong phase angle for the delta connection. Closing delta onto that mismatched flux produces a short current and torque transient, which a poorly tuned timer or a slow contactor makes worse.

### Can a star delta starter be used on any motor?

It works on any standard induction motor wound for delta running, but it only suits loads with a low starting torque requirement, since starting torque in star drops to about a third of the full-voltage figure. A load needing strong starting torque can stall the motor in the star connection before it ever reaches delta.

### Does the starting method affect what size generator I need?

Yes. Reducing starting current with a star delta starter or soft starter reduces the step load the generator has to absorb, which is often the real constraint on sizing where large motors run off a genset. The generator sizing guide linked above covers how to check a starter's current draw against a set's rated step load acceptance.

### Is it safe to adjust a star delta starter's timer myself?

No, not without the right training and an isolation and permit to work in place. The cabinet carries live three-phase power at currents that can cause serious injury, and a wiring error at the star-delta interlock can produce a short circuit across two phases, so this work should go to a qualified electrical technician.
