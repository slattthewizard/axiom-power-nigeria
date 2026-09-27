---
meta_title: "Steam Turbine Working Principle Explained"
meta_description: "Steam turbine working principle explained: impulse vs reaction, condensing vs back-pressure, main parts and where these turbines run in Nigerian plants."
primary_keyword: "steam turbine working principle"
secondary_keywords: "types of steam turbine, impulse vs reaction turbine, steam turbine parts, steam turbine components, steam turbine applications Nigeria"
---

# How a Steam Turbine Works: Principle, Types and Main Parts

A steam turbine looks simple from the outside: a long cylindrical casing, a shaft running through it, steam pipes in at one end and out at the other. What happens inside that casing is what a maintenance manager actually needs to understand, because every alarm on the panel, from low condenser vacuum to high axial displacement, traces back to how steam does its work on the blading. This article sets out the steam turbine working principle in plain terms: how steam is converted into shaft rotation, the difference between impulse and reaction staging, how condensing and back-pressure machines are built for different jobs, the main parts a technician will actually handle, and where these machines run in Nigerian industry.

Steam turbines are less common than diesel or gas gensets on the ground in Nigeria, but they sit at the centre of some of the country's largest and most technically demanding plants: combined-cycle IPPs, refineries, and sugar or palm oil mills that generate their own power from process steam. Anyone specifying, inspecting or troubleshooting one benefits from knowing the machine at this level before reading a vendor report or a vibration trend.

## The steam turbine working principle: converting heat into rotation

A steam turbine is a heat engine that follows the Rankine cycle: water is boiled into high pressure, high temperature steam in a boiler or a heat recovery steam generator (HRSG) behind a gas turbine, and that steam is expanded through the turbine to do mechanical work before it is condensed back to water and returned to the boiler feed system.

Inside the casing, the expansion happens in stages. Steam first passes through a set of stationary nozzles or a nozzle ring, which convert the pressure and thermal energy of the steam into a high velocity jet. That jet strikes the moving blades fixed to the rotor, and the change in the steam's velocity and direction as it crosses the blade produces a force on the blade, which turns into torque on the shaft. The steam leaves each stage at lower pressure and velocity than it entered, and the process repeats across many stages until the steam reaches the exhaust, either to a condenser under vacuum or to a process header at a controlled back-pressure.

Admission of steam into the turbine is controlled by governor valves that respond to load and speed demand from the control system, in the same way a genset's governor meters fuel to hold frequency. This is the basic principle behind every industrial steam turbine, regardless of size, and it is the reason a plant engineer troubleshooting a trip should start by asking what happened to steam conditions (pressure, temperature, flow) just before the event, not only what the electrical protection recorded.

## Impulse and reaction stages: the two ways blades extract energy

Turbine designers extract energy from expanding steam in one of two ways, and most industrial machines use a mix of both across their stages.

In an impulse stage, the entire pressure drop for that stage happens across the stationary nozzles. The moving blades see no further pressure change: they simply redirect the high velocity jet and absorb its kinetic energy, similar in principle to how a jet of water striking a curved bucket does work without any pressure difference across the bucket itself. Impulse blading is symmetrical and comparatively simple to manufacture, which is why smaller and older industrial sets, and the high pressure end of larger machines, often use multiple impulse stages (commonly described as Rateau or Curtis staging).

In a reaction stage, the pressure drop is shared between the stationary blades and the moving blades. The moving row is shaped like a small aerofoil, and steam expanding across it generates a reaction force in the direction of rotation in addition to the impulse effect, much as a rotating lawn sprinkler is pushed round by the reaction of the water leaving its arms. Reaction blading is more efficient at handling the larger volumetric flows found in the lower pressure end of a turbine, but it produces higher axial thrust, which is why the low pressure stages of a large machine need a substantial thrust bearing and a well-maintained oil system.

| Feature | Impulse stage | Reaction stage |
|---|---|---|
| Where the pressure drop happens | Across the stationary nozzles only | Shared across stationary and moving blades |
| Blade shape | Symmetrical profile, redirects a high velocity jet | Aerofoil profile, generates lift and reaction thrust |
| Typical location in the machine | High pressure end, and the whole of smaller sets | Lower pressure stages of larger multi-stage machines |
| Axial thrust on the rotor | Lower | Higher, needs a larger thrust bearing |

## Condensing turbines versus back-pressure turbines

The other major classification has nothing to do with the blading and everything to do with what happens to the steam after it leaves the last stage. A condensing turbine exhausts into a condenser held under vacuum, which lets the machine extract the maximum possible energy from the steam and is the arrangement used where the only product wanted is electrical power. A back-pressure turbine exhausts into a process steam header at a positive pressure set by whatever downstream process needs that steam, trading some power output for usable process heat.

The choice between the two, and the hybrid extraction designs that sit between them, matters enormously for how the machine is operated and protected, and for what a vibration or thrust trend actually means at a given load. This is covered in full in our dedicated comparison of [condensing and back-pressure turbines](/blog/back-pressure-vs-condensing-turbine/), which plant engineers specifying or inheriting a machine should read alongside this one.

## The main parts of a steam turbine

Whatever the staging or the exhaust arrangement, the components a maintenance team actually deals with are broadly the same:

- The rotor and blading, the rotating assembly that carries the moving blades and transmits torque to the coupling
- The casing or cylinder, the pressure-retaining shell that houses the stationary nozzles, diaphragms and blade rings
- Glands and seals at each point the shaft passes through the casing, which control steam leakage and, on condensing machines, air ingress into the vacuum space
- Journal bearings that support the rotor's weight, and a thrust bearing that locates the rotor axially against the steam forces described above
- The governor and control valves, plus the trip and overspeed protection system, which together manage steam admission and shut the machine down safely on a genuine fault
- The lubrication oil system, which cools and lubricates the bearings and, on larger machines, also operates the hydraulic control gear
- The coupling to the driven equipment, whether that is a generator, a compressor or a pump

Every one of these is a wear item with its own inspection interval and its own failure signature, which is why a generic service schedule copied from another machine class is a poor substitute for the OEM manual for the specific turbine on site.

## Where steam turbines run in Nigerian plants

Steam turbines are not a common sight on a factory rooftop the way diesel gensets are, but they are central to a smaller number of larger and more critical Nigerian sites.

The country's grid includes both steam-only thermal stations and combined-cycle stations. A combined-cycle plant pairs one or more gas turbines with an HRSG that recovers heat from the gas turbine exhaust to raise steam, which is then expanded through a steam turbine as a bottoming cycle, adding output without burning extra fuel. Nigeria's largest single generating station, on the Lagos lagoon, runs entirely on steam turbines fed by conventional boilers, and several of the gas-fired stations in Rivers State pair gas turbines with a steam turbine in a combined-cycle configuration in exactly this way. For how the gas turbine side of that pairing works, see our companion piece on the [gas turbine working principle](/blog/gas-turbine-how-it-works/).

Outside the grid, steam turbines also appear in Nigerian refineries, where they drive large pumps and compressors directly off extracted or exhaust process steam, and in sugar and palm oil mills, where bagasse or fibre-fired boilers raise steam that is expanded through a back-pressure turbine to generate power on site while still delivering low pressure steam to the process. In every one of these settings, the turbine is a long-life, high-value asset that is expected to run for years between major overhauls if it is looked after correctly, which is a very different maintenance relationship from a diesel genset that is serviced on running hours.

## What typically fails on an industrial steam turbine

Most steam turbine problems trace back to a handful of mechanisms, and recognising the pattern early is what keeps a fault from becoming an outage.

Bearing failure is one of the most common, usually from oil contamination, loss of oil film at low load or during startup, or long-term babbitt fatigue; our piece on [turbine bearing and babbitt failure](/blog/turbine-bearing-babbitt-failure/) goes through the mechanisms and warning signs in detail. Blade damage shows up as erosion from wet or carryover steam, corrosion pitting, deposits that unbalance the rotor, or in rarer cases fatigue cracking, and it is usually first picked up as a shift in vibration or a drop in stage efficiency rather than anything visible from outside the casing. Gland and seal wear lets steam leak out or, on the vacuum side of a condensing machine, lets air leak in, and both show up first as a slow deterioration in performance before they become an obvious fault. Rotor vibration itself, whether from misalignment, imbalance, rubbing, or a bearing problem, is worth understanding on its own terms, and our dedicated article on [high vibration on a steam turbine](/blog/steam-turbine-high-vibration/) covers the diagnostic approach.

Governor and control valve sticking, and thermal stress from rushed startups or shutdowns that heat or cool the casing and rotor unevenly, round out the common list. Any work that involves opening the casing, isolating steam or electrical supplies, or entering the rotating equipment envelope must be carried out by qualified personnel under a lockout/tagout procedure and a permit to work; this is not a machine class where an unqualified team should attempt hands-on diagnosis.

Routine inspection intervals, and what a borescope or an open inspection is actually looking for, are set out in our guide to [turbine inspection intervals](/blog/turbine-inspection-intervals/). Getting the inspection cadence right, and acting on what it finds before a minor finding becomes a forced outage, is the single biggest lever a plant has over the lifetime cost of a steam turbine. If your plant is due a condition assessment or a scoped overhaul, our engineers can review the machine's history and current condition and put together a technical proposal; see our [steam and gas turbine overhaul](/steam-turbine-overhaul-nigeria/) service, or [request a technical proposal](/#contact) directly.

## Frequently Asked Questions

### What is the basic working principle of a steam turbine?

A steam turbine expands high pressure steam through stationary nozzles and moving blades in a series of stages, converting the steam's thermal and pressure energy first into velocity and then into torque on the rotor. The steam leaves each stage at lower energy than it entered, and the cumulative effect across all the stages drives the shaft.

### What is the difference between an impulse and a reaction turbine?

In an impulse design the pressure drop happens entirely across stationary nozzles, and the moving blades only redirect the resulting jet. In a reaction design the pressure drop is shared between stationary and moving blades, and the moving blades generate additional force from the reaction of the steam expanding across them, which also produces more axial thrust on the rotor.

### What are the main parts of a steam turbine?

The core parts are the rotor and blading, the pressure-retaining casing, the stationary nozzles and diaphragms, shaft seals or glands, journal and thrust bearings, the governor and control valve system, the lubrication oil system, and the coupling to whatever equipment the turbine drives.

### Where are steam turbines used in Nigeria?

Steam turbines run in Nigeria's larger power stations, including steam-only thermal plants and the steam side of combined-cycle gas stations, as well as in refineries and in sugar and palm oil mills that raise steam from process boilers to generate power on site while also supplying process heat.

### How often should a steam turbine be inspected?

Inspection intervals depend on the specific machine, its duty cycle and the OEM manual, and typically combine continuous condition monitoring with periodic open inspections or borescope checks at intervals the manufacturer or the maintenance history justifies. A plant should build its own schedule from the OEM documentation rather than borrowing an interval from a different machine or a different site.
