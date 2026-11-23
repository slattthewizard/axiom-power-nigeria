---
meta_title: "Shaft Alignment: Methods, Tolerances and Soft Foot"
meta_description: "How shaft alignment works on plant machinery: offset and angular misalignment, dial and laser methods, soft foot, thermal growth and a safe procedure."
primary_keyword: "shaft alignment"
secondary_keywords: "laser shaft alignment, shaft alignment tolerance, coupling alignment, soft foot"
---

# Shaft Alignment: Why Misalignment Kills Bearings, Seals and Couplings, and How to Fix It

Ask a maintenance crew why a pump keeps eating mechanical seals and you'll hear about seal quality, dry running, dirty product. All fair. But if the same machine has been through three seals and two sets of bearings in a year, look at the coupling before you look at the catalogue. Shaft alignment is the cheapest bit of precision work on a plant, and it's the one most often done by eye, in a hurry, at the end of a long shutdown.

This guide covers what misalignment actually is, what it does to the parts that fail first, how it shows up in vibration, the methods used to correct it, and the checks that have to happen before anyone touches a dial indicator. It applies to motors driving pumps, fans and compressors, and to turbine and engine drives where the numbers are less forgiving.

## Offset and angular misalignment

Two shafts joined by a coupling can be wrong in two ways, and in practice they're nearly always wrong in both at once.

Parallel misalignment, also called offset, means the two shaft centrelines are parallel but don't sit on the same line. One is higher, lower or off to one side. Angular misalignment means the centrelines cross at an angle, so the coupling halves open up like a wedge on one side. You can measure both in the vertical plane (up and down, corrected with shims) and in the horizontal plane (side to side, corrected by moving the machine).

A flexible coupling doesn't cure either one. It tolerates a small amount of misalignment so the machine survives start-up and some movement in service, but every bit of that tolerance gets paid for in extra load on the bearings. Think of the coupling as a safety margin, not a licence.

## What misalignment does to the machine

The shaft has to bend or the coupling has to flex every revolution, and the energy goes somewhere. Usually it goes into three places.

Bearings take a cyclic side load that the design never intended. Rolling element bearings fatigue early, and the damage starts on the loaded zone of the race. On sleeve bearings, including the babbitt bearings on turbines, you'll see the wear concentrated on one side of the shell, with the oil film thinned where the shaft is pushed hard against it. The same mechanism sits behind many [turbine bearing babbitt failures](/blog/turbine-bearing-babbitt-failure/), though misalignment is rarely the only factor.

Mechanical seals suffer because the shaft no longer runs true through the seal faces. The faces are lapped flat to a tiny fraction of a millimetre, so any wobble opens a gap on every turn. The result is leakage, face chipping, and a seal that "just doesn't last" however many times it's replaced. If that sounds familiar, read the notes on [mechanical seal failure](/blog/mechanical-seal-failure/) and check the alignment record before you order another one.

Couplings run hot, wear their elastomer elements or grid, fret the hub bores and eventually crack or throw a bolt. A coupling guard full of black dust from a spider insert is a very honest indicator. So is a coupling that's warm to the hand with the machine running.

There's also a quieter cost. Misaligned machines draw more current for the same duty, because some of the motor's torque is spent fighting the coupling. Nobody sends a bill for that, which is partly why it goes unnoticed.

## How it shows up in vibration

Misalignment has a recognisable signature, though no single reading proves it.

The classic pattern is high vibration at 1x running speed and often at 2x, the second harmonic. Pure offset tends to push up the radial readings at 2x. Angular misalignment tends to show as high axial vibration, measured along the shaft, usually at 1x and sometimes 2x. A rule of thumb used on site: if the axial reading at a bearing is large compared with the radial reading, suspect angular misalignment, and expect phase to be roughly 180 degrees apart across the coupling.

Unbalance also produces 1x, which is why people get this wrong. Unbalance mostly shows in the radial direction and the phase readings across the coupling behave differently. Looseness adds harmonics beyond 2x. Don't diagnose from one number on one bearing. A proper vibration survey, with trended data, will usually settle it, and it's one of the practical payoffs of a [predictive maintenance](/blog/predictive-maintenance/) programme.

## Before you align: soft foot, pipe strain and the base

Alignment readings are worthless if the machine moves when you tighten it down. So the first job isn't alignment at all.

Soft foot means one foot of the machine isn't sitting flat on its base. When you tighten the hold-down bolt, the casing distorts, and the shaft moves with it. Align a machine with soft foot and you've aligned it only until the next time somebody loosens a bolt. Worse, the distortion can bind the bearings or close up internal clearances.

To check for soft foot, with the machine isolated and the coupling disconnected or the dial indicator set up on the shaft, loosen one foot bolt at a time and watch the indicator. Movement beyond the figure given in the machine maker's instructions or in your site standard means that foot needs correcting. Typical causes are a bent or dirty foot, stacked shims that have corroded or compressed, a warped baseplate, or a rocking pair of feet where the machine sits on two diagonal corners. Fix it with proper shims, and don't use more shims in a stack than you have to, because every extra layer is a spring.

Pipe strain is the other one that catches people out. If the suction or discharge flanges don't line up with the pipework and the bolts are forcing them together, the pipe is pulling the casing out of position. Check it by watching the indicator while you loosen the flange bolts one at a time. Pump people see this all the time, and it's worth reading alongside the [centrifugal pump guide](/blog/centrifugal-pump-guide/) if you're sorting out a pump installation.

Also check the base itself. Cracked grout, a loose or hollow-sounding baseplate, and corroded anchor bolts will undo any amount of careful shimming. Get these sorted first.

## Alignment methods compared

The table below sets out the methods you'll meet on site, with what each is genuinely good for.

| Method | How it works | Good for | Limits |
|---|---|---|---|
| Straightedge and feeler gauge | A straightedge across the coupling rims checks offset, feeler gauges check the gap between faces | Rough pre-alignment, getting a machine close before precision work | Not precise enough for final alignment. Affected by coupling face and rim errors |
| Dial indicator, rim and face | One indicator reads the rim (offset), another reads the face (angle) as both shafts turn together | Short couplings and small machines where you can't mount a reverse setup | Face readings are sensitive to axial float and end play. Needs good bar rigidity |
| Dial indicator, reverse dial | Two indicators read the rim of each shaft, rotated together or in turn, which gives offset and angle at both machines | Most general industrial alignment, including long spacer couplings | Bracket sag must be allowed for. Takes practice and care with the sums |
| Laser shaft alignment | Sensors and laser emitters on each shaft, measured through rotation (often only part of a turn), with the system calculating corrections | Final alignment on most machines, hot alignment checks, and where documentation is needed | Needs a clean line of sight, stable mounting and a sensible setup. Garbage in still gives garbage out |

Honestly, the equipment matters less than the discipline. A careful crew with reverse dials will beat a hurried one with a laser. That said, laser shaft alignment is faster, shows live corrections as you move the machine, and gives you a printed record, which is useful when you want to compare this year's alignment with last year's. It also handles sag and axial float better than most dial setups.

## Tolerances: use the maker's figures

Shaft alignment tolerance isn't a single number. It depends on running speed, on the coupling type, on the spacer length, and on what the machine maker allows. Tolerances tighten as speed rises, so a 3,000 rpm machine needs a finer result than a slow one, and a high-speed turbine train is tighter again.

For that reason, work from the machine manufacturer's instruction manual. If there's no manual, use a published alignment tolerance table for the speed range, such as those supplied by alignment system makers or found in industry standards, and write down which table you used. Don't quote a "standard" figure from memory, and don't trust a tolerance passed down on a site whiteboard.

Two further points. First, check the coupling maker's allowance too, because the coupling and the machine can have different limits and you work to the tighter one. Second, aim well inside the tolerance rather than scraping within it. A result at the edge of the limit leaves no margin for the changes that happen once the machine is running.

## Thermal growth on hot machines

Machines don't stay at workshop temperature. A steam turbine, a pump on hot service or a boiler feed pump heats up, and the casing and bearing housings grow. Steel expands by roughly 12 micrometres per metre for every degree Celsius it warms, which sounds like nothing until you apply it.

Take a hypothetical pump where the shaft centreline sits 400 mm above the foot and the casing runs 100 degrees Celsius above ambient. That's roughly half a millimetre of vertical rise, taken from the casing alone. If the driver stays cool, the two shafts go out of line the moment the pump warms up.

The answer is to align cold with a deliberate offset, so the machines come into line at operating temperature. The target figures come from the manufacturer, who knows how each machine grows. On turbines they're usually specified as cold offsets on the bearing housings and casings, and for hot service pumps in the instruction manual. Where the maker gives no figure, your options are to measure the movement on a first heat-up using a hot alignment check, or to get the machine assessed by someone who has done it before.

The reverse also applies: don't "correct" a hot machine to zero when the maker wants it to sit offset. Cold alignment targets and hot alignment checks go hand in hand. For turbine trains, thermal growth sits alongside many of the causes of [steam turbine high vibration](/blog/steam-turbine-high-vibration/), though that page isn't a substitute for the manual.

## A practical procedure

This is an outline, not a method statement. Your site procedure and the machine manual take priority.

1. Get a permit to work and isolate the driver. That means electrical lockout-tagout at the motor starter or breaker, or fuel and start isolation on an engine or turbine, with your own lock and tag on it. Prove it dead, and isolate and tag any process valves on pumps and compressors. Nobody turns a coupling by hand on a machine that could start.
2. Clean the feet, shims, baseplate and bolts. Record the existing shims and any condition you find.
3. Pre-align roughly with a straightedge and feeler gauges.
4. Check and correct soft foot on each foot, and note pipe strain.
5. Set up your measurement system (dials or laser), rotate the shafts, and record readings. Check that the readings repeat.
6. Calculate the vertical shim changes and horizontal moves, including any thermal growth offset specified by the maker.
7. Move the machine, tighten, and re-measure. Expect two or three passes.
8. Check the final result against your tolerance, and record it.
9. Refit the coupling guard, remove locks and tags in the right order, and close the permit.
10. Run the machine, check vibration and bearing temperature, and for hot machines, take a hot alignment check where practicable.

Dowel the machine only after you're satisfied, because dowels fix a mistake in place.

If you'd rather hand the job to a team that does this daily, our [rotating equipment services](/rotating-equipment-services-nigeria/) cover alignment, vibration checks and recommissioning as part of overhaul work.

To arrange an alignment check, a vibration survey or a full coupling inspection on your plant, [request a technical proposal](/#contact) and our engineers will scope it with you.

## Frequently Asked Questions

### How often should shaft alignment be checked?

There isn't a fixed interval that suits every plant. Check alignment after any work that moves the machine, such as a rebuild, motor change, baseplate repair or pipework change, and when vibration trends show a rise at 1x or 2x. Many sites also add it to the routine for critical machines at planned shutdowns. If you trend your vibration data, the machine will usually tell you when it's time.

### Is laser shaft alignment always better than dial indicators?

Not automatically. Laser systems are quicker, give live feedback and produce a record, so they're usually the better choice for final alignment on important machines. But a competent crew using reverse dial indicators can reach very good results, and dials work in places where a laser's line of sight is awkward. The bigger errors tend to come from soft foot, pipe strain and sloppy setup, not from the choice of tool.

### Can I fix misalignment by buying a more flexible coupling?

You can hide it for a while, but you won't fix it. A more flexible coupling transmits less of the misalignment load, so the machine may run quieter at first, though the bearings and seals still carry whatever the coupling can't absorb. Every flexible coupling has a stated misalignment capacity, and that's the limit for occasional movement, not a target for installation. Align the machine properly and the coupling lasts longer.

### What's the difference between soft foot and pipe strain?

Both distort the machine and spoil alignment, but the source differs. Soft foot comes from the machine's own feet not sitting flat on the base. Pipe strain comes from the connected pipework forcing the casing out of position. You check soft foot by loosening each foot bolt in turn, and pipe strain by loosening the flange bolts while watching an indicator. Fix soft foot first, since you can't measure pipe strain reliably on a machine that rocks.

### Does a new machine need alignment, or does the maker do it?

Always check. Factory alignment, where it exists, doesn't survive transport, lifting and installation on a different base. Grouting, anchor tightening and connecting the pipework all move the machine. Treat the delivered condition as a starting point, and align the machine in its final position with the pipework connected.
