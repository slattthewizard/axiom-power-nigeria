---
meta_title: "Soft Starter Guide: How It Works and When to Use One"
meta_description: "How a soft starter works, how to set ramp time and current limit, and when to pick it over DOL, star-delta or a VFD, including on generator-fed sites."
primary_keyword: "soft starter"
secondary_keywords: "soft starter vs vfd, soft starter for motor, soft starter vs star delta, motor starting methods"
---

# Soft Starter Guide: How It Works, How to Set It and When It Beats DOL, Star-Delta or a VFD

A big induction motor started direct on line takes six to eight times its full-load current for a second or two, and it does it with a bang you can feel in the floor. The lights dip, the governor hunts, and the coupling and gearbox pay for it over time. A soft starter takes most of that violence out of the start without changing the motor.

This guide covers how a soft starter works, what the ramp and current-limit settings do, why the bypass contactor matters in a hot Nigerian MCC room, and how it compares with the other motor starting methods. It also covers the thing generator-fed sites care about most: how much smaller a set you can get away with.

## How a soft starter works

Inside a soft starter, each phase has a pair of thyristors (SCRs) wired back to back, one pointing each way. A thyristor only conducts when the control board fires its gate, and the board can fire it late in each half-cycle. Fire it late and only a slice of the sine wave reaches the motor, so the effective voltage is low. Fire it earlier and earlier on each cycle and the voltage climbs.

That's the whole trick. The starter begins at a set starting voltage, often 30 to 40 percent of line voltage, and ramps it up over a few seconds until the motor sees full voltage. Current follows voltage, and torque follows voltage squared, so the motor accelerates gently instead of being thrown at the load.

One thing is worth understanding before you touch a setting. The motor is not being fed a clean sine wave during the ramp, so there's some extra heating in the motor and some harmonic content in the supply while the thyristors are chopping. Once the motor reaches speed the thyristors are fully on and the starter has done its job, which is where the bypass comes in.

## Ramp time, starting voltage and current limit

Most industrial soft starters give you three main adjustments, and they interact.

Initial voltage (or initial torque) sets where the ramp begins. Too low and the motor just hums while the load sits still, wasting seconds of heating with no motion. Too high and you've lost the point of the exercise. A sensible start is the lowest value at which the shaft begins to turn within a second or so.

Ramp time sets how long the voltage takes to reach full value. A pump might be happy with 5 to 10 seconds, a heavy fan 20 to 30. Longer isn't better: if the load hasn't accelerated by the end of the ramp, you get a sudden jump when full voltage arrives anyway.

Current limit caps the starting current at a chosen multiple of full-load current, typically somewhere between 2 and 4 times. The starter holds the voltage at whatever level keeps current at that cap until the motor speeds up. This is the setting that matters on generators, because it puts a hard number on your starting kVA.

Honestly, the commonest mistake is a long ramp with no current limit on a load that needs real breakaway torque. The motor stalls at partial voltage, the overload trips, and the soft starter gets blamed. Start with a current limit and a modest ramp, and watch the actual start before tuning further.

Set the motor nameplate current in the starter before anything else, because the overload protection works from it.

## The bypass contactor and heat in a hot MCC room

Thyristors drop roughly a volt or so each when conducting. Multiply that by the motor current and you get heat. As a rough rule, a soft starter running continuously dissipates around 3 watts per amp across its three phases. A 200 A motor means something like 600 W of heat sitting inside the starter for as long as it runs. That's a small heater in a cabinet.

Over a 10-second start that's nothing. Over a 24-hour run in an already hot MCC room it's a problem. That's why most soft starters either have an internal bypass contactor or need an external one. When the ramp ends, the bypass contactor closes across the thyristors, the current flows through the contactor contacts instead, and the heat load drops to almost nothing. The starter stays connected for protection and for a soft stop if you've enabled it.

For Nigerian sites, think about ambient temperature honestly. Many soft starters are rated for 40 degrees Celsius without derating, and an MCC room with poor ventilation, dust-clogged filters and no air-conditioning can sit well above that on a Harmattan afternoon or in the wet-season humidity. Check the derating curve, keep the heatsink fins clear, and don't mount a starter above a heat source in the cabinet. If you can't hold the room temperature down, a bypass is not optional.

Treat the bypass as part of the starter, not an extra. A starter with no bypass and no cooling, running a pump 24/7, will eventually cook itself.

## Soft starter vs DOL, star-delta and VFD

Here's how the main motor starting methods compare in practice. Cost is given as a relative class only.

| Method | Starting current | Starting torque | Speed control | Harmonics | Cost class |
|---|---|---|---|---|---|
| DOL (direct on line) | 6 to 8 times full-load | Full, with a hard kick | None | None | Low |
| Star-delta | About 2 to 2.5 times full-load, with a second transient at changeover | Roughly one third of DOL | None | None | Low to medium |
| Soft starter | Adjustable, typically 2 to 4 times full-load | Reduced and smooth, falls with the square of voltage | None, only start and stop ramps | Some during the ramp only | Medium |
| VFD | About 1 to 1.5 times full-load | Can hold full torque at low speed | Full range | Continuous, needs attention | High |

DOL is fine when the motor is small compared with the supply. The problem starts when it's large relative to the source, which on a generator is sooner than people think.

Star-delta cuts the starting current to roughly a third of the DOL value, but it has no adjustability, and the changeover from star to delta creates its own current spike and torque jerk. We cover that properly in [the star-delta starter article](/blog/star-delta-starter/). In a soft starter vs star delta decision, the soft starter wins on smoothness and on having a tunable limit, and star-delta wins on simplicity, no electronics and a low cost class.

A VFD is a different animal. It controls the frequency as well as the voltage, so you get speed control, a starting current close to full-load and full torque at low speed. If the process benefits from running at varying speed, [the variable frequency drive guide](/blog/variable-frequency-drive-guide/) is where to look. For a gentle start on a fixed-speed motor a VFD is usually overkill. If you regularly run a fan or pump well below full flow, the VFD pays you back in energy and the soft starter can't.

## Why soft starters help on generator-fed sites

This is where the soft starter earns its place in Nigeria. A diesel set doesn't have the stiffness of the grid. When a large motor starts DOL the generator sees a huge kVA demand for a moment, voltage sags, frequency dips, and the AVR and governor fight to recover. Sag deep enough and other loads drop out, contactors chatter, and the motor itself may fail to accelerate.

Take a hypothetical 160 kW motor, starting a fixed load. Started DOL at about six times full-load current, its starting demand is very roughly six times the running kVA, which the generator has to supply instantly. With a soft starter holding current to about three times full-load, that demand is roughly halved. Because the generator's transient capability is the real constraint, that can mean the difference between needing a much larger set and getting by with one that's sized for the running load plus some margin.

You still can't size on running kW alone: the voltage dip must stay inside what other loads tolerate, and torque is reduced too. Work through the sums properly, using [the generator sizing guide](/blog/generator-sizing-guide/), and include the starting method in the calculation instead of assuming DOL.

The thyristor chopping adds some distortion during the ramp. It's short-lived, but see [the power system harmonics article](/blog/power-system-harmonics/) if your bus already carries VFDs, UPS units or rectifiers.

## Limitations: when a soft starter is the wrong answer

A soft starter is not a universal fix.

It gives no speed control. It starts and stops the motor smoothly, and that's it. If you need the motor at 60 percent speed, you need a VFD.

Starting torque is reduced, and the reduction is steep because torque falls with the square of voltage. At 50 percent voltage you have about a quarter of DOL torque. A loaded conveyor or a compressor starting against pressure may need more breakaway torque than a low current limit allows.

High-inertia loads need care. Large fans, centrifuges and flywheel-driven machines accelerate slowly, and a long start at 3 times full-load current heats the motor and the thyristors. Check the motor's permitted start time and the starter's duty rating. A 40-second start probably needs a heavy-duty model.

Frequent starts are another trap. Each start dumps heat into the motor windings, so count starts per hour against the ratings.

Finally, it won't help with a motor that's already unhealthy. If a motor trips on overload during the start, check the winding insulation first with a megger test before blaming the starter settings.

## Commissioning and safety

Any work inside the starter panel, on the bypass contactor or at the motor terminals needs the circuit isolated, locked out and tagged out, with a permit to work in place. Prove dead with a tester, because control supplies and capacitors can hold charge. Afterwards, record the initial voltage, ramp time, current limit and the measured start current and time. When something drifts, that record is the first thing you'll want.

If you're sizing starters for a plant or a generator-fed site and want a second opinion on the starting method, [request a technical proposal](/#contact) or book a plant assessment, and our engineers will look at the loads, the supply and the room the equipment sits in.

## Frequently Asked Questions

### What is the difference between a soft starter and a VFD?

A soft starter only controls voltage during the start and stop, then the motor runs at line frequency and fixed speed. A VFD changes both voltage and frequency, so it can run the motor at any speed, hold torque at low speed and start with almost no inrush.

### Is a soft starter better than star-delta?

For most motors, yes, because you can adjust the current limit and ramp, the start is smooth, and there's no open-transition spike at changeover. Star-delta is still fine for light-start loads where simplicity matters and there's no electronics in a hot room.

### Can a soft starter reduce the generator size I need?

It can. By limiting starting current to a few times full-load instead of six to eight, it lowers the starting kVA the generator must supply, which can allow a smaller set or reduce the voltage dip when a big motor starts. You still have to check the voltage dip and the torque the load needs.

### Do I need a bypass contactor on a soft starter?

For any motor that runs for long periods, yes. Without a bypass, the thyristors carry full motor current continuously and dissipate heat the whole time, which is a real problem in a hot MCC room. A bypass contactor takes over once the motor is at speed.

### Can a soft starter be used on any motor?

It suits standard three-phase squirrel-cage induction motors with a reasonable starting torque requirement. It's a poor fit for loads needing high breakaway torque at low voltage, very high-inertia loads without a heavy-duty rating, and applications with very frequent starts.
