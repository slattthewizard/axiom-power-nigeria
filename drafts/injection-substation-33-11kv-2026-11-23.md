---
meta_title: "33/11kV Injection Substation: Equipment and Upkeep"
meta_description: "What a 33/11kV injection substation does in the Nigerian network, why industrial users take supply at 33kV or 11kV, and the equipment and maintenance involved."
primary_keyword: "33/11kv injection substation"
secondary_keywords: "injection substation, 33/11kv substation equipment, industrial substation nigeria, dedicated feeder"
---

# 33/11kV Injection Substation: What It Does, What's Inside and How Industrial Users Work With It

If you run a large plant in Nigeria, you've probably heard someone say "we're on a dedicated 11kV feeder off the injection substation" and nodded along. It's worth knowing what that sentence actually means, because the substation at the other end of your cable decides how often your plant sees the grid, how clean that supply is, and how fast anyone can fix a fault.

A 33/11kV injection substation is the point where sub-transmission voltage is stepped down to the distribution voltage that feeds towns, industrial estates and individual factories. It sits downstream of the transmission company's bulk stations and upstream of the small pole-mounted and ground-mounted transformers that bring the voltage down to 415 V. This article explains where it fits, why heavy users want to connect close to it, what equipment you'll find inside, and what has to be maintained.

## Where the Injection Substation Sits in the Network

The Nigerian grid has three broad layers. The Transmission Company of Nigeria (TCN) operates the high voltage network and the transmission stations, typically stepping down to 33kV at the bulk supply points. From there the distribution companies (DISCOs) take over. They carry power on 33kV lines to injection substations, step it down to 11kV, and run 11kV feeders out to distribution transformers, which finally give 415 V to the end user.

So the injection substation is the DISCO's main interface to the lower voltage network. One 33kV incomer (often two, in a better arranged station) feeds one or two power transformers, and the secondary side of those transformers feeds a bank of 11kV feeder breakers. Each feeder serves a geographic area or a specific load.

## Why Large Industrial Users Take Supply at 33kV or 11kV

Most small businesses take supply at 415 V from a shared distribution transformer. A plant drawing a few megawatts can't sensibly do that. The cables would be enormous, the losses high, and the transformer would be shared with neighbours whose loads you don't control. So bigger users connect at 11kV or, for the largest loads, at 33kV, and own or lease their own step-down transformers on site.

There are three practical reasons, and they're the ones plant managers actually care about.

First, a dedicated feeder. When your plant is the only customer, or one of very few, on an 11kV feeder, a fault on somebody else's street doesn't trip your supply. Shared feeders in the distribution network are tripped by faults, overloads and load shedding decisions that have nothing to do with you. A dedicated feeder removes most of that exposure. It also usually means your feeder breaker is a known, identifiable device, so there's a name to ask about when the supply drops.

Second, supply hours. Tariff bands such as Band A are designed around higher expected availability, and the feeders that serve those customers tend to be the ones the DISCO protects. A dedicated industrial feeder is the most natural way to give a Band A customer the availability the band is meant to carry. The exact supply obligations and any compensation terms are set by the regulator and your supply agreement, so check the current requirement with NERC and your DISCO rather than relying on what someone remembers from a meeting. For the cost side of this, see our piece on [Band A tariff versus self-generation](/blog/band-a-tariff-vs-self-generation/).

Third, voltage quality. A long, heavily loaded 415 V or shared 11kV network droops under load. Motors run hot, drives trip on undervoltage, and sensitive process equipment misbehaves. Close to the injection substation, the on-load tap changer on the power transformer is actively holding the 11kV bus voltage, so what you receive is steadier.

## What Is Inside a 33/11kV Injection Substation

On the 33kV side you have incoming lines, isolators, circuit breakers and surge protection. The power transformer sits in the middle. On the 11kV side there's a switchboard with an incomer, a bus section if the board is split, and a row of feeder breakers. Behind all of it is the part nobody sees from the road: protection relays, the battery that keeps them alive, the earthing grid and the metering.

The table below sets out the main items and what each does.

| Equipment | What it does |
|---|---|
| 33kV incoming isolators | Provide a visible, lockable break so crews can work on equipment without the line being live. They aren't designed to break load current. |
| 33kV circuit breakers | Interrupt load and fault current on the incoming side, operated by protection relays or manually. |
| Lightning arresters | Divert lightning and switching surges to earth before they damage the transformer winding or switchgear insulation. |
| Power transformer with on-load tap changer | Steps 33kV down to 11kV. The tap changer adjusts the turns ratio under load to hold the 11kV voltage steady as demand changes. |
| 11kV switchgear and incomer | Receives the transformer output and distributes it across the busbar. |
| 11kV feeder breakers | One per outgoing feeder. Isolate a faulted feeder without taking down the others. |
| Protection relays | Detect overcurrent, earth fault, differential and other abnormal conditions and send trip signals to the breakers. |
| Current and voltage transformers (CTs and VTs) | Scale primary current and voltage to safe, small values for relays and meters. |
| Station battery and DC system | Supplies trip coils, closing circuits, relays and control power when the AC supply is lost. |
| Earthing grid | Gives fault current a low resistance path to ground and keeps touch and step voltages within safe limits. |
| Metering | Records energy and demand at the billing point, and is where the DISCO and the customer's figures meet. |

A couple of these deserve a closer look. The on-load tap changer is the only part of the transformer that regularly moves under electrical stress, so it's the most common source of transformer trouble. And the battery system is the quiet single point of failure of the whole station. If the DC supply is dead, a breaker may refuse to trip when a fault arrives, and a small fault becomes a large one.

## How the Power Transformer and Tap Changer Behave

The transformer's job sounds simple: take in 33kV, put out 11kV. In practice the load changes by the minute, and the incoming voltage wanders with the state of the upstream network. Without a tap changer, the 11kV side would follow it up and down.

An on-load tap changer lets the transformer change its ratio in small steps while carrying load. The automatic voltage control relay watches the 11kV bus and tells the tap changer to step up or down when the voltage leaves its set band. That's why the voltage at a well run injection substation holds better than at the end of a long feeder.

It also means the tap changer is working all day. Contacts wear, the diverter switch oil carbonises, and the mechanism needs attention on a schedule. Transformer oil is the thing that tells you the most about the machine's health, which is why oil sampling comes up in every maintenance plan. We cover testing and diagnosis in [transformer maintenance](/blog/transformer-maintenance/).

## Coordination With the DISCO and TCN

Here's where a lot of plants get stuck, and it's mostly paperwork and communication, not engineering.

The injection substation itself normally belongs to and is run by the DISCO. The upstream 33kV supply may come from a TCN station. Your plant takes its supply at a defined point of connection, and everything on your side of that point is your responsibility. What sits on which side, who may operate which switch, and who pays for what are set by your connection agreement and the applicable regulations. We don't quote those here, and you shouldn't take anybody's word for them. Read your agreement, and check the current rules with the regulator. The Electricity Act 2023 changed some of the structure around who may generate, distribute and contract for supply, and we've summarised what it means for plants in [Electricity Act 2023 for industrial users](/blog/electricity-act-2023-industrial-users/).

A few practical habits help.

- Agree in writing who authorises switching on the feeder, and keep the control room contact list current.
- Keep your protection settings coordinated with the DISCO's upstream relays. If your incomer trips slower than theirs, their breaker takes the feeder down for a fault inside your plant.
- Record every trip with a time stamp and the relay flags. Those records settle arguments about whose fault it was.

When the grid itself collapses, the injection substation de-energises and your feeder goes with it. What your plant does at that moment, and what happens when the supply returns in a surge, is a separate subject covered in [grid collapse and plant protection](/blog/grid-collapse-plant-protection/).

## Maintenance Items That Actually Matter

Anything below that involves working on or near energised or recently energised plant needs isolation, lockout-tagout and a permit to work, with the circuit proved dead and earthed before anyone touches it. At 33kV and 11kV there's no such thing as a quick look.

Transformer oil comes first. Sample it on a schedule, and test for moisture, acidity, breakdown voltage and dissolved gases. Gas patterns can show overheating or arcing inside the tank long before anything trips. Oil leaks, silica gel breathers that have turned colour and Buchholz relay gas collections are all things a walk-round should catch.

Tap changer servicing follows the manufacturer's schedule, whether it's set by operation count or by time. Don't stretch it because the voltage looks fine. The failure mode is a contact that overheats and welds, and it gives little warning.

Circuit breakers need their operating mechanisms checked, timing tests done and contacts inspected, as the maker specifies. A breaker that hasn't operated for months can stick, and that's the day you need it.

Protection relays should be tested on a regular cycle: secondary injection to confirm settings and trip times, and a functional trip test through to the breaker. Relay settings drift in the paperwork more than in the hardware. Make sure what's on the relay matches the current protection study.

Earthing resistance gets measured and the connections inspected, especially after any ground works or theft. Cable and strap theft is a real problem on some sites. A grid that has lost a few joints can look fine and still fail to carry a fault current.

The station battery and charger need checking at intervals: float voltage, electrolyte levels where applicable, cell condition, and a discharge test to prove the battery can actually carry the load. A charger on float and a battery at the end of its life look the same until the AC goes.

If you need a second pair of eyes on your incoming supply arrangement, protection settings or substation maintenance plan, [request a technical proposal](/#contact) and our engineers will scope it with you.

## Frequently Asked Questions

### What's the difference between a 33/11kV injection substation and a distribution substation?

An injection substation steps 33kV down to 11kV and feeds several 11kV feeders. A distribution substation sits further downstream, usually on one of those feeders, and steps 11kV down to 415 V for end users. The injection station is larger, has more protection and typically serves many thousands of customers through its feeders.

### Why would a factory want its own dedicated feeder?

A dedicated feeder means faults and load shedding on neighbouring areas don't automatically take your plant offline. It also gives steadier voltage and a clear point to point to when supply drops. Whether you can get one depends on your load, your DISCO and your connection agreement.

### Who maintains the equipment, the DISCO or the customer?

It depends on where the point of connection is. The DISCO normally maintains the injection substation and the feeder up to that point. The customer maintains everything on its own side, including incoming switchgear and plant transformers. Check your connection agreement for the exact boundary.

### How often should substation protection relays be tested?

There's no single answer. Many operators follow the relay manufacturer's guidance and their own protection policy, and test after any settings change or major fault. Whatever interval you choose, test through to the breaker, not just the relay, and keep the records.

### Does a 33/11kV supply remove the need for standby generation?

No. A dedicated feeder cuts the number of outages but doesn't remove upstream faults, grid collapses or planned shutdowns. Most plants on 11kV or 33kV still keep standby generation sized for the loads that can't stop.
