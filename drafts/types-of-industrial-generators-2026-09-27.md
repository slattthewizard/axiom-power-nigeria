---
meta_title: "Types of Industrial Generators: A Nigeria Buyer's Guide"
meta_description: "A plant manager's guide to the types of generator used across Nigerian factories, hospitals, banks and telecoms sites: fuel, duty rating, speed, enclosure."
primary_keyword: "types of generator"
secondary_keywords: "types of generators and their uses, diesel vs gas generator, standby vs prime generator, industrial generator types"
---

# Types of Industrial Generators: A Business Buyer's Guide for Nigeria

Search for the types of generator and most of what comes back is written for a homeowner choosing between a small petrol set and an inverter generator for the weekend. That is not the decision a plant manager, facility engineer or procurement officer in Nigeria is making. The question at factory, hospital, bank or telecoms site scale is which combination of fuel, duty rating, speed, enclosure and control configuration fits a specific load, run pattern and site, and industrial generator types are classified along several of those axes at once, not one.

This guide sets out the classifications that actually drive a specification: fuel type, duty rating, running speed, enclosure, alternator and excitation type, and single-set versus synchronised multi-set configuration. Each one answers a different question, and a real specification is built by combining them, not by picking a single category and stopping there.

## Classifying by Fuel: Diesel, Gas, CNG, LPG and Dual Fuel

Fuel type is the classification most buyers start with, because it decides what supply infrastructure the site needs and how the maintenance programme is structured.

**Diesel generators** remain the default across Nigerian industrial and commercial sites because diesel is available almost everywhere, storage and handling are well understood, and the engines tolerate a wide range of duty cycles. The trade-offs are fuel storage, security against theft and adulteration, and exposure to the pump price and exchange rate, covered in more detail in the [diesel generator price](/blog/diesel-generator-price-nigeria/) guide.

**Natural gas generators** run on pipeline gas or CNG and suit a site with reliable gas supply nearby, typically industrial clusters around Lagos, Port Harcourt and the Niger Delta. Gas quality (methane number, moisture, hydrogen sulphide content) has to be checked against the engine manufacturer's specification, since an engine designed for one gas composition can derate or misfire on another. The [gas generator guide](/blog/gas-generator-guide/) covers fuel supply routes and gas quality in full.

**LPG generators** are less common at large industrial scale in Nigeria but appear on smaller sets and as a top-up fuel where CNG or pipeline gas is not economic to bring in.

**Dual fuel and bi-fuel generators** are a separate category from a purpose-built gas set. A dual-fuel conversion lets a diesel engine burn a gas and diesel blend, using diesel as the pilot fuel that ignites the mixture, and is usually chosen where an existing diesel fleet needs to reduce diesel consumption without a full re-engine. A bi-fuel set, by contrast, can run on either fuel but not a blend of the two at once, giving supply flexibility rather than a cost-driven blend ratio. Both differ in complexity, control strategy and maintenance burden from a factory-built gas engine, and the conversion route needs an engineering assessment of the specific base engine before it is chosen.

## Classifying by Duty Rating: Standby, Prime and Continuous

Duty rating answers a different question from fuel type: how many hours a year is the set expected to run, and at what load factor.

A **standby-rated** set is built and sized to cover an outage on an otherwise reliable supply, for a limited number of hours a year, at a lower average load factor than a prime-rated machine of the same nameplate output. A **prime-rated** set is expected to run for unlimited hours as the primary source of power, typically at a defined average load factor over its duty cycle, with an allowance for periodic overload. A **continuous-rated** set carries a constant, unvarying load with effectively no allowance for overload, closer to a baseload power plant application than a backup role.

The confusion that costs money is running a standby-rated set as if it were prime rated, which is common in Nigeria given how many hours a year mains supply is unavailable at some sites. That shortens engine and alternator life, can void a manufacturer warranty, and is worth understanding before a set is bought. The [standby vs prime generator rating](/blog/standby-vs-prime-generator-rating/) article sets out the rating classes and the practical effect of running a set outside its intended duty.

## Classifying by Speed: 1500 rpm and 3000 rpm

Engine speed is a classification buyers often overlook until they compare two quotes for the same kVA figure and find very different machines behind them.

A **1500 rpm set** (a four-pole alternator on a 50 Hz supply) turns more slowly, which generally means a longer engine life, lower mechanical wear per unit of output, and a larger, heavier package for a given kVA rating. **3000 rpm sets** (two-pole alternators) run at double the speed, giving a lighter, more compact and often lower-cost package for the same rated output, at the expense of a shorter typical service life and higher wear rate over comparable running hours.

The practical rule of thumb followed across most industrial specifications is that 1500 rpm sets suit prime and continuous duty, where total running hours over the machine's life are high, and 3000 rpm sets suit standby duty, where the set runs comparatively few hours a year and the lighter, cheaper package matters more than long-run durability. A [generator sizing](/blog/generator-sizing-guide/) exercise should settle the duty rating and expected annual running hours before speed is chosen, not after.

## Classifying by Enclosure: Open, Soundproof and Containerised

Enclosure type is driven by where the set sits and what is around it, not by the engine or alternator inside.

**Open-type sets** have no acoustic enclosure and are the cheapest and simplest option, suited to a dedicated generator room, a remote compound, or any location where noise and weather exposure are not constraints.

**Soundproof canopy sets** wrap the engine and alternator in an acoustic enclosure with a weatherproof skin, reducing noise output for sites near occupied buildings, residential boundaries or noise-sensitive operations such as a hospital ward or a bank branch. Noise limits and the units they are measured in are covered in the [generator noise emission limits](/blog/generator-noise-emission-limits/) piece.

**Containerised sets** go a step further, housing the generator, fuel system and sometimes switchgear inside a purpose-built or modified shipping container, giving a self-contained, relocatable unit suited to sites with limited covered space or a need to move the asset between locations. Containerised units carry their own ventilation, fire suppression and access considerations that a simple canopy does not.

## Classifying by Alternator and Excitation: Self-Excited and PMG

The alternator's excitation system decides how the set behaves under fault conditions and under the kind of non-linear electrical load common on modern industrial and commercial sites.

A **self-excited (brushless, shunt or compound) alternator** draws its excitation power from its own output windings through an automatic voltage regulator, which is simple and cost-effective but means the excitation supply weakens as the machine's own output collapses during a downstream short circuit, limiting how much fault current it can sustain to trip protective devices cleanly.

A **PMG (permanent magnet generator) excited alternator** carries a small permanent-magnet generator on the same shaft, supplying the AVR independently of the main output windings. That gives more stable voltage regulation under harmonic-rich, non-linear loads such as variable frequency drives, UPS systems and switch-mode equipment, and it sustains a higher fault current for longer during a short circuit, which matters for correct operation of downstream circuit breakers. A bank, data centre or hospital running sensitive electronic loads is the more likely candidate for a PMG-excited set; a straightforward mechanical or resistive load on a factory floor may not need the added cost.

## Configuration: Single Set and Synchronised Multi-Set

The final classification is not about the machine itself but how many of them work together.

A **single-set configuration** is the simplest: one generator sized to cover the site's peak demand, with the usual margin for starting current and future growth. It is straightforward to control and maintain but concentrates risk in one machine, and any planned or unplanned outage on that set removes the entire backup capacity.

A **synchronised multi-set configuration** parallels two or more generators onto a common bus, sharing load between them under a synchronising and load-sharing controller. This spreads risk across machines, allows sets to be taken out for maintenance without losing all standby capacity, and lets total running capacity track actual demand rather than sitting at one large machine's fixed output. The trade-off is a more complex control and protection scheme, including synchronising checks, reverse power protection and load-sharing logic, and the maintenance discipline needed to keep every set in the group in a condition where it will synchronise reliably when called on. The mechanics of paralleling gensets are covered separately; the classification point here is that multi-set operation is a distinct design choice from simply buying a bigger single machine.

## Matching Generator Type to the Facility

None of these classifications is chosen in isolation. A factory, a hospital, a bank branch and a telecoms site each combine them differently because their load profiles, outage tolerance and site constraints differ.

| Facility | Typical duty need | Common configuration |
|---|---|---|
| Factory (process load) | Prime, often high annual hours given grid unreliability | 1500 rpm, single set or synchronised multi-set depending on load and redundancy needs |
| Hospital | Standby with very low tolerance for transfer delay | 1500 rpm preferred for critical loads, PMG excitation for sensitive equipment, often multi-set for redundancy |
| Bank branch or data hall | Standby to prime depending on branch size, sensitive to voltage quality | Soundproof canopy, PMG excitation for non-linear IT and UPS loads |
| Telecoms site | Standby, remote and often unmanned | Containerised or soundproof canopy, sized for high reliability with minimal site visits |

The right combination for any one site still depends on its actual load, run-hour pattern and growth plans, which is why a load study and sizing exercise, not a category label, should set the final specification. For ongoing servicing once a set is chosen and installed, see [industrial generator and genset maintenance](/generator-maintenance-nigeria/), and to have a load profile and site conditions assessed against these classifications, [request a technical proposal](/#contact).

## Frequently Asked Questions

### What is the difference between a diesel and a gas industrial generator?

A diesel generator uses compression ignition and runs on widely available diesel fuel, while a gas generator uses spark ignition on pipeline gas, CNG or LPG and needs a gas supply route and gas quality checks that a diesel set does not. The choice depends more on fuel availability at the specific site than on a general preference for one technology.

### Is a 1500 rpm or 3000 rpm generator better for a factory?

For a factory running as prime power with high annual running hours, a 1500 rpm set is usually the better fit because of its longer expected service life at a given output. A 3000 rpm set suits a lighter standby role where annual running hours are low and the smaller, lower-cost package matters more.

### What type of generator is best for a hospital?

A hospital typically needs a standby-rated set with fast, reliable transfer and stable voltage for sensitive medical and IT equipment, which often points to a 1500 rpm set with PMG excitation, sized with enough margin and redundancy to keep critical loads covered if one unit is down for maintenance. The exact specification still depends on the hospital's actual load profile.

### Do I need a synchronised multi-set system instead of one large generator?

Not always. A single large set is simpler to run and maintain, and suits a site that can tolerate its backup capacity being fully offline during planned maintenance. A multi-set synchronised system suits a site that cannot accept that risk, or whose load varies enough that running several smaller units efficiently makes more sense than one oversized machine.

### Does the enclosure type affect generator performance?

Not directly. Open, soundproof canopy and containerised enclosures are about noise control, weather protection and site placement rather than the engine or alternator's electrical performance, though a poorly ventilated enclosure of any type can cause the set to derate on cooling grounds, which is a design and installation issue rather than a feature of the enclosure category itself.
