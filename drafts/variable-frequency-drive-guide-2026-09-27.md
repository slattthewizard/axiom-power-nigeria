---
meta_title: "Variable Frequency Drive (VFD) Guide for Plant Engineers"
meta_description: "A plant engineer's guide to variable frequency drives in Nigeria: how VFDs cut energy use on pumps and fans, manage harmonics, and what fails."
primary_keyword: "variable frequency drive"
secondary_keywords: "vfd, vfd working principle, vfd for pumps and fans, vfd harmonics, motor starting methods"
---

# Variable Frequency Drives (VFDs) for Pumps and Fans: A Plant Engineer's Guide

If your plant runs centrifugal pumps or fans at full speed and controls flow with a throttle valve or a damper, you are paying to make power and paying again to throw part of it away. A variable frequency drive changes that by varying the motor's speed instead of fighting it downstream. For a facility running its own generators or gas turbines, that has a direct effect on fuel burn, genset loading, and the life of the motors themselves.

This guide sets out how a VFD works, where it earns its keep on pumps and fans, what it does to power quality, and what keeps one running in Nigerian plant conditions: heat, dust and long duty cycles. It also covers common faults and when a VFD is the wrong tool for the job.

## How a variable frequency drive works

A variable frequency drive controls the speed and torque of an AC induction motor by changing the frequency and voltage supplied to it, rather than running the motor directly off the fixed 50 Hz supply. The basic VFD working principle has three stages. A rectifier converts the incoming AC supply to DC. A DC bus, usually with capacitors, smooths that DC and stores a small amount of energy. An inverter section, built from power transistors (typically IGBTs), switches the DC back into AC at whatever frequency and voltage the application needs, using pulse width modulation to approximate a sine wave.

Because motor speed is tied to supply frequency, for a fixed number of poles, controlling frequency controls speed. Voltage is varied alongside frequency to keep the motor's magnetic flux, and therefore its torque capability, roughly constant across the speed range. A built-in controller handles start and stop ramps, current limiting and protection functions, and most industrial drives also carry overload protection and a set of digital and analogue inputs for tying into a plant control system.

## VFD for pumps and fans: where the savings actually come from

Centrifugal pumps and fans are the classic case for a VFD, because their load follows the affinity laws. Flow varies directly with speed, but power varies with the cube of speed. Cut a fan or pump's speed by 20 per cent and flow drops by roughly the same 20 per cent, but the power it draws drops by close to half. That is a much bigger saving than closing a valve or a damper, both of which waste energy as friction or turbulence rather than cutting it at the source.

Take a hypothetical example with no site attached to it: a cooling water pump sized for a peak duty that only occurs a few hours a day, running the rest of the time throttled back with a valve. Fitted with a VFD and controlled from a pressure or flow signal instead, the pump only turns as fast as the process actually needs. The saving is real physics, not a promised percentage, and the actual figure depends on the duty curve and how much of the time the machine runs below full load. A power plant audit is the right way to establish whether a given pump or fan is a good VFD candidate before spending on one; see /power-plant-audit-nigeria/ for how that assessment is scoped.

Beyond the energy bill, a VFD reduces mechanical shock. Starting a motor across the line pulls several times rated current for a few seconds and slams the pump or fan up to full speed almost instantly. A drive ramps the motor up over a set time, which is gentler on couplings, bearings, seals and the driven equipment, and avoids the pressure spikes that a direct-on-line pump start can put through a pipe network.

## VFD harmonics and the effect on your generator

The rectifier front end of a standard VFD does not draw a smooth sine-wave current from the supply. It draws current in pulses, which introduces harmonic distortion, most of it at the 5th and 7th harmonics for a typical six-pulse drive. On a large public grid this is usually absorbed without much drama. On a plant running its own generators, or a captive gas turbine set, it is a different matter, because the source impedance is higher and the generator has far less capacity to soak up distorted current than a national grid connection does.

The practical effects on a genset feeding VFD loads include extra heating in the alternator windings, distorted voltage waveform that can upset the AVR's sensing and cause hunting, and, in bad cases, nuisance tripping or overheating of the generator itself. This gets worse as the ratio of VFD load to total generator capacity rises, which is exactly the situation on a plant running mostly VFD-driven pumps, fans and compressors off one or two sets. Size the generator and the drive together at the design stage, using the derating guidance in the generator's own datasheet and the drive manufacturer's harmonic data; see /blog/generator-sizing-guide/ for the wider sizing questions this feeds into.

Mitigation options, in rough order of cost, include a drive with a higher pulse count front end (12-pulse or active front end) for the larger loads, line reactors or harmonic filters, and spreading large VFD loads across more than one generator where the plant has that flexibility. A total harmonic distortion limit is normally written into the generator or utility specification, and standards bodies such as IEEE publish recommended practice for harmonic control in electrical power systems; the specific limit for a given installation should be confirmed against the generator manufacturer's data, not assumed.

## Specifying and sizing a VFD

A drive is matched to the motor's rated current and voltage, and to its kW rating, because two motors of the same power can draw different current depending on efficiency and power factor. Beyond the motor nameplate, the specification should cover:

- Duty type: constant torque (conveyors, some compressors) versus variable torque (centrifugal pumps and fans), since the drive's overload and cooling requirements differ between the two.
- Ambient temperature and altitude at the installation, since drives derate in hot enclosures.
- Enclosure rating for a dusty or humid plant room, and whether the drive will sit in an air-conditioned panel room or an ordinary factory environment.
- Control interface: what signal drives the speed reference (a 4 to 20 mA transmitter, a fieldbus link, a plant SCADA point).
- Braking requirement: whether the load needs dynamic braking or can coast to stop.

An undersized drive nuisance-trips on overcurrent under real load; an oversized one costs more and can be less accurate at low speed. The manufacturer's sizing tables, applied against the motor nameplate and duty cycle, are the reference point, not a rule of thumb from an unrelated application.

## Keeping a VFD running: cooling, dust and capacitors

A VFD is an electronic device operating in an environment that is often hot and dusty, and both conditions shorten its life if the drive is not kept clean and cool.

Heat is the main enemy of the power semiconductors and the DC bus capacitors. Every drive has a maximum ambient rating, and running above it accelerates capacitor ageing and can trigger thermal trips under load. Panel rooms with failed air conditioning or blocked ventilation louvres are a common, avoidable cause of drive failures on Nigerian sites.

Dust is the second problem, especially during harmattan. Dust on heatsinks and cooling fans reduces airflow, which raises internal temperature even where the room itself is not particularly hot, and dust that is conductive or hygroscopic raises the risk of tracking faults on the control board. Filters on ventilated enclosures need scheduled cleaning, not a reactive clean-out after a trip.

DC bus capacitors have a service life measured in years rather than decades, and that life shortens with heat and ripple current, both higher on heavily loaded drives in hot rooms. Manufacturer manuals typically call for a capacitor check or replacement on a multi-year interval, and some drives log capacitor condition internally, worth reading at a scheduled service rather than only at failure. Cooling fans inside the drive are also wear items with a rated life and should be replaced on schedule rather than run to failure, since a fan failure often takes the drive down with it.

## Common VFD faults

| Symptom | Likely cause | What to check |
|---|---|---|
| Drive trips on overcurrent at start | Mechanical binding, wrong motor parameters, ramp time too short | Load is free to turn, motor nameplate data matches drive parameters, acceleration ramp |
| Drive trips on overvoltage during stop or deceleration | Load decelerating faster than the drive can absorb the regenerated energy | Deceleration ramp time, whether a braking resistor or dynamic braking is fitted |
| Drive runs hot or shows a thermal fault | Blocked ventilation, dirty heatsink, ambient above rating, undersized enclosure cooling | Fan operation, heatsink and filter cleanliness, panel room temperature |
| Erratic speed or nuisance faults on generator power | Voltage distortion or sag from the generator, poor AVR response under VFD load | Generator loading and voltage waveform, whether other VFD loads are running on the same set |
| Ground fault trip | Insulation breakdown in motor windings or cable, moisture ingress | Insulation resistance test on motor and cable (see the note on safety below) |
| No display, drive will not power up | Blown control fuse, failed control power supply, tripped upstream protection | Incoming supply and fuses, control transformer, upstream breaker |

Any check that involves opening a drive enclosure, testing motor insulation, or working on the associated switchgear needs a qualified electrical technician working under a permit to work with proper lockout/tagout. VFD DC buses hold a dangerous charge for some time after the supply is switched off, and this is not work for an unqualified person to attempt live.

## VFD versus other motor starting methods

A VFD is not the only way to reduce starting current or control a motor. Star-delta starters and soft starters both cut starting current for a fixed period during start-up, then run the motor at full speed on the line, with no ongoing speed control. A VFD costs more but gives continuous variable speed, the affinity-law saving described above, and a controlled ramp on every start and stop, not only the first few seconds. Where a load genuinely runs at one speed most of the time, a soft starter or star-delta arrangement may be the more cost-effective choice; see /blog/star-delta-starter/ for how that comparison plays out and what it means for step loads on a generator.

For a plant weighing up a new drive installation, a VFD for pumps and fans, or which loads are worth converting first, our engineers can scope the assessment against your pump and fan curves, generator capacity and duty cycles. Request a technical proposal through /#contact, or start with /rotating-equipment-services-nigeria/ for how pump, fan and rotating equipment work is typically structured.

## Frequently Asked Questions

### Does a VFD reduce electricity use even if the motor still runs most of the time near full speed?

The saving on a VFD comes mainly from time spent below full speed, because power falls with the cube of speed on a centrifugal load. A pump or fan that genuinely runs close to full speed nearly all the time will show a smaller saving than one that spends significant hours throttled back, so the duty cycle matters more than the motor's rated power.

### Can a VFD be added to an existing motor, or does the motor need to be replaced?

Most standard induction motors can run on a VFD without modification, provided the drive is matched to the motor's voltage, current and duty type. At very low speeds a standard motor's own cooling fan turns slowly and may not move enough air, which matters for continuously loaded applications and is usually addressed with a separately powered cooling fan or by limiting the minimum speed.

### How many VFDs can one generator or gas turbine set safely support?

There is no single fixed ratio, because it depends on the drive's pulse count, the generator's source impedance and its own harmonic tolerance, and how much of the total load is non-VFD. This is a sizing exercise for the specific generator and drive combination, done against manufacturer data, not a rule that carries across different installations.

### What is the difference between a VFD and an inverter?

In plant engineering the two terms are largely interchangeable when talking about a device that converts fixed-frequency AC to variable-frequency AC for motor control. Some manufacturers use "inverter" as their product name for what is functionally a VFD, and some use "inverter" more narrowly for the switching section inside the drive.

### Do VFDs need any special maintenance beyond what the motor itself needs?

Yes. The motor still needs its own bearing and insulation checks, but the drive itself is an electronic enclosure with cooling fans, filters and DC bus capacitors that age with heat and running hours, and these need their own inspection and replacement schedule separate from the motor's mechanical maintenance.
