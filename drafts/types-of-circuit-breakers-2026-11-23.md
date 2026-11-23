---
meta_title: "Types of Circuit Breakers: MCB, MCCB, ACB, VCB, SF6"
meta_description: "Types of circuit breakers by voltage and arc-quenching medium: MCB, MCCB, ACB, vacuum, SF6 and older oil breakers, with selection and testing points."
primary_keyword: "types of circuit breakers"
secondary_keywords: "types of circuit breaker and their uses, mcb mccb acb, vacuum circuit breaker, sf6 circuit breaker"
---

# Types of Circuit Breakers: MCB, MCCB, ACB, Vacuum and SF6 Explained for Plant Engineers

Walk through any industrial site in Nigeria and you'll find breakers from three or four different generations sitting within a hundred metres of each other. A modern moulded case unit in the generator panel, an air breaker in the main LV board, and somewhere in the substation a medium voltage breaker that may be vacuum, may be SF6, and may be an oil-filled relic nobody wants to talk about. Knowing the types of circuit breakers on your site, and what each one needs, is basic housekeeping for a maintenance manager.

A circuit breaker does two jobs. It carries load current without complaint, and it opens a faulty circuit quickly enough that the fault current doesn't destroy the equipment downstream. The hard part is the second job. When contacts part under fault current, an arc forms, and the breaker's design is really a design for killing that arc. That's why the most useful way to classify breakers is by voltage class and by the medium that extinguishes the arc.

## How Circuit Breakers Are Classified

There are three sensible ways to sort them. By voltage: low voltage (up to 1 kV), medium voltage (roughly 1 kV to 36 kV) and high voltage above that. By arc-quenching medium: air, oil, vacuum or SF6 gas. And by construction: miniature, moulded case, open (air) frame, and the metal-clad switchgear types where the breaker racks in and out of a cubicle.

In practice the first and second ways collapse into each other. Low voltage breakers quench the arc in air using arc chutes. Medium voltage is where vacuum took over from oil, and SF6 is common at the top end of medium voltage and everywhere above it. So the working list for most plants is MCB, MCCB and ACB on the low voltage side, then vacuum and SF6 on the medium voltage side, plus whatever older oil and air-blast units are still in service.

## Low Voltage Breakers: MCB, MCCB and ACB

These three cover everything from a single socket circuit to the incomer of a large generator board. People mix up the names, so here's the short version.

An MCB (miniature circuit breaker) is the small DIN-rail unit in distribution boards. It usually goes up to around 125 A, with breaking capacity typically in the 6 to 10 kA range for standard units. It has a fixed trip characteristic, so you can't adjust it, and it's meant for final circuits: lighting, sockets, small motors, control supplies.

An MCCB (moulded case circuit breaker) is the sealed, box-shaped breaker you see on sub-distribution boards and motor control centres. Ratings run from about 100 A up to roughly 1,600 A, sometimes more. Breaking capacity is much higher than an MCB, commonly from 16 kA into the 100 kA range depending on the frame. Smaller MCCBs are thermal-magnetic, and larger ones usually have an electronic trip unit with adjustable settings.

An ACB (air circuit breaker) is the big open-frame breaker, normally draw-out, found on main incomers, bus couplers and generator outgoing circuits. Ratings start around 800 A and go up to 6,300 A. ACBs are built to be maintained: you can rack one out, open the arc chutes, and inspect or replace contacts. They also carry a short-time withstand rating, which lets them stay closed for a short period during a downstream fault so a smaller breaker nearer the fault can clear it first. That's what makes proper selectivity possible.

## Medium and High Voltage: Vacuum and SF6 Circuit Breakers

Once you're at 11 kV or 33 kV, which is where most Nigerian industrial plants take their supply or distribute internally, the breaker is almost always a vacuum or SF6 design.

A vacuum circuit breaker (VCB) puts the contacts inside a sealed ceramic bottle held at a very high vacuum. With almost no gas to ionise, the arc dies out at the first current zero. VCBs are compact, have a short stroke, need very little maintenance, and are the standard choice from about 3.3 kV up to 33 kV or so. The thing that kills them is a bottle losing its vacuum. You can't see that by looking, which is why a periodic vacuum integrity test matters.

An SF6 circuit breaker uses sulphur hexafluoride gas, which is a very good arc-quencher and insulator. SF6 breakers appear at the upper end of medium voltage and are the default across high voltage, from 33 kV through transmission levels. The gas is also used in gas-insulated switchgear (GIS), which packs a substation into a fraction of the floor space, useful on cramped sites. The catch is that SF6 is a powerful greenhouse gas and its arc by-products are toxic, so it must never be vented and needs trained handling.

Honestly, for new medium voltage work in a typical plant the choice is rarely close. Vacuum wins below about 36 kV on simplicity and low maintenance. SF6 earns its place where the voltage is higher or the space is tight.

## Older Types Still Found in Nigerian Substations

You'll still meet oil and air-blast breakers in older substations, including some inside industrial plants built decades ago.

A bulk oil circuit breaker has its contacts submerged in a tank of insulating oil. The arc decomposes the oil, producing hydrogen that helps quench it. They're heavy, they carry a fire risk, and the oil needs regular testing and changing. A minimum oil breaker does the same job with far less oil, in small interrupter chambers, which cuts the fire risk and the maintenance load but doesn't remove them. Neither is made for new installations any more, and finding spares gets harder every year.

Air-blast breakers store compressed air and blow it across the contacts to chase the arc out. They were used at high voltage in earlier decades, and they're noisy and need a compressed air plant to keep working. If you find one, you're looking at a candidate for replacement or retrofit, not a long-term asset.

The practical advice on all three is the same: don't assume they're safe because they still close. Their fault-clearing performance degrades with age, their protection relays are often equally old, and a retrofit with a vacuum unit in the same cubicle is frequently cheaper in risk terms than another round of oil changes. A proper [power plant audit](/power-plant-audit-nigeria/) should put every one of these breakers on the asset register for exactly that reason.

## Typical Voltage Range and Use by Breaker Type

The ranges below are textbook typical values. The nameplate on your own breaker is the only number that counts.

| Breaker type | Typical voltage | Typical current range | Where you'll find it |
|---|---|---|---|
| MCB | Up to 440 V AC | About 0.5 to 125 A | Final circuits, lighting, small loads |
| MCCB | Up to 690 V AC | About 100 to 1,600 A | Sub-distribution, motor feeders, generator outgoing on smaller sets |
| ACB | Up to 690 V AC | About 800 to 6,300 A | Main incomers, bus couplers, large generator breakers |
| Vacuum (VCB) | About 3.3 to 36 kV | Up to around 4,000 A | 11 kV and 33 kV plant switchgear, motor starters, transformer feeders |
| SF6 | About 11 kV to 800 kV | Wide range | Upper medium voltage, high voltage, GIS |
| Bulk and minimum oil | About 3.3 to 132 kV | Varies | Legacy substations, mostly being phased out |
| Air-blast | About 11 to 400 kV | Varies | Historic high voltage stations |

## Selection Points: Current, Breaking Capacity, Trip Unit, Selectivity

Picking a breaker by its ampere rating alone is the classic mistake. Four things need to line up.

Rated current. Size it to the load and the cable it protects, remembering that a breaker in a hot, enclosed Lagos switchroom carries less than its catalogue figure. Derate for the ambient, not the brochure.

Breaking capacity. This is the highest fault current, in kA, that the breaker can interrupt safely, and it must exceed the prospective fault level at the point of installation. It's the number people forget. When a site adds a new transformer or a bigger generator, the fault level at the main board rises, and breakers that were fine last year can end up under-rated. Check it again after every significant change to the supply.

Trip unit. A thermal-magnetic unit uses a bimetal strip for overload and a magnetic coil for short circuits. It's simple and cheap, and the settings are mostly fixed or have a narrow adjustment. An electronic trip unit measures current with sensors and gives you adjustable long-time, short-time and instantaneous settings, sometimes earth fault protection and metering as well. For anything on a main incomer or a generator, electronic is the sensible choice. If you're feeding a motor, our guide to the [star-delta starter](/blog/star-delta-starter/) explains why the instantaneous setting has to ride over the starting current.

Selectivity. When a fault occurs, only the breaker closest to it should trip. That depends on the upstream breaker having a higher setting or a deliberate time delay, and on both being coordinated on a time-current chart. Poorly coordinated boards trip the whole plant for a fault on one pump motor. That's a downtime cost nobody budgets for.

Also check how the breaker fits the rest of the system. A generator breaker that interlocks with the mains breaker is the whole point of a transfer scheme, so the way it behaves matters for your [automatic transfer switch and AMF panel](/blog/automatic-transfer-switch-amf-panel/).

## Maintenance and Testing

Breakers sit doing nothing for months and then have to work in a few cycles. A breaker that hasn't operated in two years may not operate on demand, so the best test is to exercise it. Everything below is hands-on work on switchgear: it needs isolation, lockout-tagout, earthing of the circuit, a permit to work, and a competent person who knows that panel.

The usual tests on a medium voltage breaker are these:

- Contact resistance, measured with a micro-ohmmeter across each closed pole. A high or rising reading points to worn or contaminated contacts, and you compare it to the manufacturer's value and the last test.
- Timing and travel, which measures closing and opening times and contact synchronism between poles. Slow or uneven operation is an early sign of a tired mechanism or a dry linkage.
- Insulation resistance, pole to earth and across open contacts, using a megger at a voltage suited to the breaker class. Our [megger insulation resistance guide](/blog/megger-test-insulation-resistance/) covers technique and interpretation.
- Vacuum integrity on a VCB, usually a high-voltage withstand test across the open bottle, following the manufacturer's method and values.
- Trip tests, checking that the protection relay and trip coil actually open the breaker. On LV electronic trip units this means a secondary or primary injection test to confirm that the pick-up and time settings match the coordination study.

Mechanism care is mostly mundane: clean and lubricate as the maker specifies, check springs and charging motors, check auxiliary contacts and the trip and close coil circuits, and confirm the racking mechanism and interlocks work smoothly. Dust and humidity do most of the damage in Nigerian switchrooms, so seals, heaters and filters are worth checking at each visit.

SF6 breakers add a few rules of their own. Gas pressure or density should be monitored and logged. Gas that needs removing is recovered with proper equipment and not vented. After an internal fault or a heavy interruption the gas and the by-product dust are hazardous, and the work needs trained people and the right protective equipment. Follow the manufacturer's handling procedure and any current regulator requirement on greenhouse gases.

Don't test the breaker in isolation. A breaker is only as good as the protection relay and the CTs driving it, and the transformer feeding it is part of the same fault path, so schedule this alongside your [transformer maintenance](/blog/transformer-maintenance/) outage rather than on its own.

If you're not sure what's installed on your site, how old it is, or whether the breaking capacity still matches your fault level, our engineers can walk the switchgear with you and tell you where the risk sits. [Request a technical proposal](/#contact) or book a plant assessment.

## Frequently Asked Questions

### What are the main types of circuit breakers?

By arc-quenching medium they are air, oil, vacuum and SF6. By use, the common ones are MCB, MCCB and ACB at low voltage, and vacuum and SF6 breakers at medium and high voltage. Oil and air-blast breakers are older designs that you'll still find in some substations.

### What is the difference between an MCB, MCCB and ACB?

The difference is mainly current rating and construction. An MCB handles small final circuits up to about 125 A, an MCCB covers roughly 100 A to 1,600 A in a sealed moulded case, and an ACB is an open-frame, draw-out breaker for main incomers from around 800 A to 6,300 A. Breaking capacity and adjustability rise at each step.

### Which is better, a vacuum circuit breaker or an SF6 circuit breaker?

For most plant switchgear below about 36 kV, vacuum is the usual pick because it's compact and needs little maintenance. SF6 makes more sense at higher voltages or where space is very limited. SF6 also brings gas handling and environmental obligations that vacuum doesn't.

### How often should circuit breakers be tested?

There's no single interval that fits every site. It depends on the manufacturer's guidance, how often the breaker operates, and the environment it sits in. Plan testing around planned shutdowns, and test any breaker that has cleared a fault before putting it back in service.
