---
meta_title: "Motor Rewinding vs Replacement: A Plant Guide"
meta_description: "Motor rewinding in Nigeria: when a rewind is the right call, what a competent rewind shop should do, and how to test the motor before it goes back on line."
primary_keyword: "motor rewinding"
secondary_keywords: "electric motor rewinding, motor rewinding nigeria, rewind vs replace motor, motor repair"
---

# Electric Motor Rewinding: When It Makes Sense and What a Proper Job Looks Like

A motor comes off a pump, fan or compressor with a burnt winding, and the plant is now running a decision under time pressure: send it out for motor rewinding, or scrap it and buy new. Get the decision wrong either way and it costs the plant twice, once in the repair or replacement itself and again in the downtime while the wrong call plays out.

Motor rewinding is a legitimate repair route for most industrial motors, not a last resort. The winding is only one part of the machine, and replacing copper and insulation on a sound core and shaft can bring a motor back to full service life. The risk sits in two places: rewinding a motor that should have been replaced, and using a rewind shop that cuts corners on the process and the testing that follows it.

This article sets out how to weigh rewind against replace, what a shop doing the job properly actually does to the core and the winding, and what tests should come back to you before the motor is refitted. None of this is step-by-step guidance for working on the motor yourself: isolation, lockout and testing on rotating electrical machinery is work for qualified personnel operating under a permit to work.

## Why windings fail in the first place

A rewind shop worth using will tell you the failure mode before it tells you the price. The common ones on industrial sites in Nigeria:

- **Thermal ageing**: insulation breaks down over years of running hot, often because the motor is oversized or undersized for the load, the cooling fins are caked in dust, or ventilation around the motor is blocked.
- **Moisture ingress**: motors standing idle in humid plant rooms, or exposed to washdown and rain, pick up moisture that drops insulation resistance and eventually breaks down under voltage.
- **Contamination**: cement, flour, oil mist or corrosive fumes get into the windings and attack the insulation directly, which is a common single-phase-to-earth fault pattern on process motors.
- **Single-phasing and voltage unbalance**: a lost phase, a loose terminal or an unbalanced supply drives extra current through the remaining windings and cooks them from the inside, usually fast.
- **Bearing currents**: on motors run from variable frequency drives, high-frequency currents induced on the shaft can pit bearings and, over time, damage the winding through repeated arcing to earth.
- **Mechanical overload or a locked rotor**: a jammed pump or fan, or a motor started against a stuck load, pulls starting current for far longer than the winding is designed to carry.

Whatever the cause, get it identified before the motor is rewound. A rewind fixes the winding, not the root cause. A motor rewound and put straight back onto the same unbalanced supply or the same blocked cooling path will fail again.

## Rewind or replace: the actual decision

The rewind-versus-replace call is an engineering and criticality decision before it is a cost comparison. Weigh these factors:

| Factor | Leans towards rewind | Leans towards replacement |
|---|---|---|
| Frame size and age | Larger frames (roughly 55 kW and above), motor still within its typical service life | Small fractional to low kilowatt motors, motor already old and near end of life |
| Core condition | Core loss test and visual inspection show a sound, undamaged core | Core shows burning, hot spots, or laminations fused from a severe fault |
| Efficiency class | Rewound to the original design with equivalent or better winding materials | Original motor is an old, low-efficiency design and a modern high-efficiency replacement is readily available |
| Criticality and spares | Motor is a common frame size held in stock elsewhere, or a spare is already on site | Motor is unique to the process and downtime cost while waiting for a rewind is unacceptable |
| Damage extent | Winding failure only, shaft, bearings and enclosure intact | Shaft bent, bearing housings damaged, or casting cracked |
| History | First failure, cause identified and corrected | Repeat failures on the same motor pointing to a chronic site problem |

A motor that has failed more than once in a short period is telling you something about the installation, not the winding. Chasing that with another rewind without fixing the supply, the loading or the cooling is a cycle that will keep repeating regardless of how good the rewind is.

On efficiency, the honest position is that a rewind done to a poor standard (excessive heat during winding removal, wrong wire gauge, poor slot fill) can measurably reduce efficiency, while a rewind done to the original design with quality materials keeps efficiency close to the original nameplate figure. If efficiency matters more than the capital cost of a new motor, for a continuously running process motor for example, that tips the balance towards a modern replacement rather than a rewind, and is a fair question to raise when scoping the work through a technical proposal.

## What a competent rewind shop does before touching the winding

Before a single coil is stripped out, the shop should record the motor's nameplate data, take insulation resistance and winding resistance readings on the existing winding, and run a core loss test (sometimes called a core imperfection or loop test) to confirm the laminations have not been damaged by the fault that took the motor out. Skipping the core test is one of the more common shortcuts, and it matters: a damaged core rewound without repair will run hot and fail again inside the new winding's life.

The old winding is then removed, ideally by a controlled burn-off oven or mechanical stripping rather than an open flame applied by hand, because excessive or uneven heat during stripping is one of the main ways a core gets damaged during a rewind rather than during the original fault.

## Winding, insulation class and impregnation

The new winding should match the original design: same wire gauge, same number of turns, same connection (star or delta), same slot fill. Changing any of these changes the motor's characteristics and can shift the current draw and torque curve away from what the driven equipment and the protection settings expect.

Insulation class should meet or exceed the motor's original rating. Many industrial motors are Class F as standard, and shops working on demanding or dusty environments will often upgrade to Class H materials for extra thermal margin, though the OEM manual for the specific motor still governs what is appropriate for that frame and duty. After winding, the stator goes through vacuum pressure impregnation (VPI): the windings are impregnated with resin under vacuum and pressure, then cured, which fills voids in the winding, bonds the coils together against vibration, and improves both the mechanical strength and the moisture resistance of the insulation system. A dip-and-bake process without the vacuum stage is a lower standard and worth asking about directly.

## Testing after the rewind, before it goes back into service

A rewound motor should not go back onto a driven load without a documented set of test results. At minimum, expect:

- **Insulation resistance (megger) test** on the new winding, corrected for winding temperature, with a comparison against the manufacturer's minimum guidance for the voltage class. See our guide to [megger testing and insulation resistance](/blog/megger-test-insulation-resistance/) for how that test is read.
- **Polarisation index** on larger motors, which trends the insulation resistance reading over time rather than relying on a single-point value.
- **Winding resistance** across all three phases, checked for balance between phases.
- **Surge comparison test**, which stresses the winding with a voltage pulse to pick up weak turn-to-turn insulation that a standard megger test will not detect.
- **No-load run test**, checking current draw, vibration and bearing temperature before the motor is coupled back to its load.
- **Temperature rise test** where the motor's criticality justifies it, run under load once installed.

Ask for the test sheet with figures, not a verbal "it passed". A shop confident in its own work will hand over the numbers without being asked twice.

## Documentation to keep on file

Once the motor is back in service, keep the rewind report with the asset record: nameplate data, the fault found, core test result, winding specification used, insulation class, and the full set of post-rewind test figures. That record is what tells the next engineer, whether that is one of ours or someone else's, whether a repeat failure is a new problem or the same one recurring, and it is also what you would hand to us if you wanted a second opinion on a rewind done elsewhere.

Rewinding and testing rotating electrical machinery involves working on and around energised or previously energised equipment, and it must be carried out by qualified personnel under lockout, tagout and a permit to work. That applies to the isolation of the motor before removal as much as to the electrical testing after the rewind.

If a motor on your site has failed and you are weighing a rewind against a full replacement, our engineers can assess the failed unit, the driven equipment and the site conditions that caused the failure as part of our [rotating equipment and compressor services](/rotating-equipment-services-nigeria/). Request a technical proposal through [our contact page](/#contact) and we will scope the assessment against your specific motor and application rather than a generic rewind quote.

## Frequently Asked Questions

### Does rewinding a motor reduce its efficiency?

A rewind done to the original design, with the correct wire gauge, slot fill and a proper vacuum pressure impregnation cycle, keeps efficiency close to the nameplate figure. Efficiency loss happens when the stripping process damages the core through excessive heat, or when the shop uses the wrong winding specification, which is why the core loss test and the winding design sheet matter more than the price quoted for the job.

### How long does a typical industrial motor rewind take?

Turnaround depends on frame size, winding complexity and whether the required insulation materials and bearings are in stock at the shop, so it is not a fixed figure across all motors. For a motor that a process cannot run without, ask the shop for a firm turnaround before committing the unit, and weigh that against holding a spare motor on site as covered in our note on spare parts lead times.

### Can any winding be rewound, or are some motors better replaced outright?

Most standard induction motors can be rewound if the core is sound. Motors that are physically damaged beyond the winding, badly obsolete, or small enough that a new unit costs little more than a quality rewind are usually better replaced. The core loss test result is the deciding factor on whether a rewind will hold up.

### What should I ask a rewind shop before sending a motor out?

Ask what core test they run before stripping the winding, what insulation class and impregnation process they use, and what test results you will receive afterwards, specifically insulation resistance, winding resistance and a no-load run. A shop that cannot answer these clearly is not one to trust with a motor that a plant depends on.

### Is a rewound motor as reliable as a new one?

Reliability after a rewind depends on the quality of the process, not on the fact that it was rewound rather than replaced. A motor rewound to the original design, with a sound core and a full set of post-rewind tests, can run as reliably as it did before the fault. What it will not fix is the underlying cause of the failure, which needs its own investigation regardless of whether the motor is rewound or replaced.
