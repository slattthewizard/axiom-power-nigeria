---
meta_title: "Generator Earthing for Industrial Plants in Nigeria"
meta_description: "A practical guide to generator earthing, neutral earthing and earth electrode resistance for industrial plants and switchboards across Nigeria."
primary_keyword: "earthing"
secondary_keywords: "generator earthing, neutral earthing, earthing system, earth electrode resistance, tn-s vs tt"
---

# Generator Earthing for Industrial Plants in Nigeria: What Actually Protects Equipment and People

Earthing on an industrial site rarely gets attention until something goes wrong: a nuisance trip that will not clear, an earth fault relay that keeps resetting itself, a technician who gets a tingle from a metal enclosure that should be dead. By then the earthing system, or the way the generator's neutral is bonded to it, is usually the reason. On plants running their own generation alongside grid power, or paralleling multiple sets, earthing decisions made at installation stage keep causing problems for years if nobody checks them again.

This is a working reference for plant managers, maintenance managers and facility engineers on what an earthing system does on their site, what a sound generator installation looks like, and where the common failures turn up on Nigerian plants: shared electrodes, corroded connections, and neutral bonding never coordinated between the genset and the incoming grid supply.

Earthing work on live switchboards and generator neutral links is not a task for unsupervised staff. Any inspection, testing or modification of an earthing or bonding arrangement should be carried out by qualified personnel under a permit to work, with the circuit isolated and locked out where the work requires it.

## Why earthing matters on a generator installation

An earthing system does two jobs on an industrial site. First, it gives fault current a low-impedance path back to source so the protective device, whether that is a fuse, an MCCB or an earth fault relay, sees enough current to trip quickly. Second, it limits the voltage that appears on exposed metal (a generator frame, a switchboard door, a motor casing) during that fault, so a person touching it is not exposed to a dangerous shock voltage for long enough to matter.

Both jobs depend on the earthing conductors and electrodes having low enough resistance and being connected the way the design intended. A generator earthed correctly as a standalone source can become badly earthed the moment it is wired into a changeover arrangement with the grid supply, because there are now two possible earth reference points and the design has to decide which one governs.

## Earthing system types: TN-S, TN-C-S, TT and IT in plain terms

Most industrial sites in Nigeria run one of four earthing arrangements, and it is worth knowing which one applies to a given switchboard before touching a generator neutral.

- TN-S: the neutral and the protective earth are kept as two separate conductors all the way from the source. This is common where a utility supply brings in a dedicated earth conductor, or where a site has its own generator earth electrode and runs separate neutral and earth conductors throughout the installation.
- TN-C-S: the neutral and earth are combined for part of the run (often called PEN) and then split into separate neutral and earth conductors at the site's main intake or distribution board. This is a frequent arrangement where a utility-style combined neutral-earth feed lands on site.
- TT: there is no earth conductor back to the source at all. Instead, the installation relies on its own local earth electrode, and protection depends on residual current devices rather than high fault current flowing back to a remote source earth. Standby generators on TT-type sites need their own local earth reference.
- IT: the source is either not earthed or earthed through a high impedance, and the installation depends on continuous insulation monitoring rather than a fast trip on the first fault. This shows up mostly in specific process areas (hospitals, some oil and gas installations) rather than general plant supply.

The table below sets out the practical difference for someone specifying or auditing a generator connection.

| System | Neutral-earth arrangement | What protects people | Where it commonly shows up |
|---|---|---|---|
| TN-S | Separate neutral and earth conductor from source | Fast trip on high fault current | Sites with a dedicated site earth electrode and generator |
| TN-C-S | Combined neutral-earth (PEN) split at intake | Fast trip on high fault current, but a broken PEN is dangerous | Utility-style intakes, many commercial buildings |
| TT | No earth conductor from source; local electrode only | RCD/RCCB operation, not high fault current | Rural or standalone sites, some generator-only installations |
| IT | Source ungrounded or high-impedance grounded | Insulation monitoring, alarm before trip | Hospitals, selected process areas |

The system in use dictates how the generator's neutral should be earthed, what protective device settings make sense, and whether an RCD is doing the real safety job or just a backup one. An OEM installation manual for the specific set, together with the site's electrical design, governs the final arrangement: this table is for orientation, not a specification to copy without checking.

## Neutral earthing when a generator runs with the grid or in parallel

The single rule that causes the most trouble on Nigerian sites is this: a system should have one, and only one, point where the neutral is bonded to earth at any time. On a plant that switches between grid supply and a generator, or that parallels two or more generators, having more than one neutral-earth bond active at once creates a path for circulating currents, some of it flowing through earth conductors, structural steel or cable armour never sized for it. Left long enough, that current heats connections, corrodes electrodes and creates nuisance earth fault trips that look like a generator problem but are actually a bonding problem.

This is why the switching device between grid and generator matters as much as the generator itself. A changeover switch or automatic transfer switch needs the correct pole configuration (three-pole or four-pole) so the neutral is switched along with the phases where the design calls for it, keeping a single neutral earth reference active at a time. Pole count, switching sequence and interlocking are covered in our guide to [changeover switch selection](/blog/changeover-switch-guide/); the same single-earth-point principle applies when two or more sets are synchronised and sharing load, covered in [generator synchronisation](/blog/generator-synchronization/).

Getting this wrong is rarely obvious from the outside. The set starts, takes load and runs. The consequence shows up later as a relay that will not reset, a genset that trips on earth fault under specific load combinations, or corrosion at an electrode that a fault survey eventually traces back to years of low-level circulating current.

## Earth electrode resistance: what it measures and why dry-season soil matters

An earth electrode, whether it is a driven rod, a grid, or a plate, only does its job if the resistance between it and the general mass of earth is low enough for the protective device to see a real fault. That resistance is not fixed. It moves with soil moisture, soil type and temperature, so a reading taken in the wet season can look acceptable and the same electrode can read several times higher once the harmattan dries the ground out.

This matters on Nigerian sites more than in temperate climates because the seasonal swing in soil resistivity is larger. An electrode that passed a test in August can fail the same test in February with nothing on the electrode itself having changed. General industry guidance tends to set a lower target for larger substation-type earths, often described as needing to be in the low single digits of ohms, and a higher ceiling for a single generator or switchboard earth pit. The number that actually applies to a given installation comes from the protective device coordination study for that switchboard, not a figure picked off a table, so treat any resistance number here as typical guidance rather than a specification.

Testing an electrode properly (fall-of-potential or a clamp-on method, done correctly) needs training and calibrated equipment, with the circuit isolated in the right sequence. Log results so a downward trend in a corroding electrode is caught before the dry season turns a marginal reading into a failed one.

## Lightning and surge bonding for gensets and switchboards

A generator installation with a lightning air termination system, and a switchboard with surge protection devices fitted, only work as designed if the earthing they rely on is bonded into the same overall system as the power earthing. A separate lightning earth electrode not bonded to the power system earth can, during a strike, sit at a very different potential to the rest of the installation for long enough to damage equipment or injure someone bridging the two systems.

Surge protection devices on a generator's output or an incoming switchboard need a short, low-impedance path to earth to clamp a transient effectively. A long or poorly terminated bonding conductor defeats much of the point of fitting the device. On sites prone to lightning activity or voltage transients from grid switching, check this bonding at the same time as the electrode resistance test, not as a separate exercise months later.

## Common earthing faults found on Nigerian industrial sites

A few patterns turn up repeatedly during plant audits and fault investigations:

- A generator sharing an earth electrode with an unrelated system (a telecoms mast, a neighbouring tenant's supply) with no coordination on fault levels or bonding.
- Corroded or loosened electrode connections, often below grade where nobody looks unless a resistance test flags it.
- A changeover switch that does not switch the neutral, leaving two neutral-earth bonds active whenever the generator is on load.
- Bonding conductors sized for the original installation but never re-checked after a load increase or an additional generator was added.
- Earth continuity broken by later civil or structural work (a slab replacement, a fence repair) that disturbed a buried conductor without anyone tracing it first.

Most of these are found on a proper earth resistance and continuity survey, not by looking at the switchboard from the front. They are also the kind of fault that a routine generator service does not necessarily catch unless earthing is explicitly on the checklist.

## Building earthing checks into the maintenance plan

Earth electrode resistance testing, bonding continuity checks and a visual inspection of accessible connections belong on a fixed interval, not an ad hoc basis after a problem shows up. A sensible baseline for most industrial sites is an annual resistance test as a minimum, done in the dry season when the reading is at its worst, with more frequent checks for sites with high soil resistivity, corrosion-prone ground, or generators that parallel or transfer between sources often. Tie the earthing check into the same visit as other electrical maintenance so a qualified technician is not on site twice for related work.

If your plant's generator earthing has never been formally tested, or if you are adding a second set, a changeover switch, or a synchronising panel to an existing installation, get the earthing arrangement reviewed as part of that scope rather than assumed. Our [generator maintenance](/generator-maintenance-nigeria/) programme includes electrical checks of this kind, and you can request a technical proposal through [our contact page](/#contact) to have a specific site assessed before or after any planned change.

## Frequently Asked Questions

### What is the difference between generator earthing and neutral earthing?

Generator earthing usually refers to the whole system of electrodes and bonding conductors connecting equipment frames and enclosures to earth for safety. Neutral earthing refers specifically to the point, or points, where the neutral conductor is bonded to that earth system. On a site with a single generator or a single incoming supply this distinction matters less, but once a generator can be switched or paralleled with another source, keeping only one active neutral-earth bond becomes the critical detail.

### How often should earth electrode resistance be tested on an industrial site?

There is no single interval that suits every site because soil condition and installation risk vary widely. An annual test done during the dry season, when resistance is typically at its highest, is a reasonable minimum for most plants, with shorter intervals for sites known to have corrosive or highly resistive soil, or generators that switch or parallel frequently.

### Can a generator use the same earth electrode as the main grid supply?

It depends on the earthing system in use and how the changeover or transfer arrangement is designed. In many configurations the generator and the incoming supply are intended to share a single earth reference, switched so that only one neutral-earth bond is active at a time. Sharing an electrode without that coordination, or without checking fault levels, is one of the more common site faults found during audits.

### What happens if a changeover switch does not switch the neutral?

If the neutral is left connected on both sides while phases are switched, two neutral-earth bonds can end up active at once. That creates a path for circulating current through earth conductors, bonding straps or structural steel that were not designed to carry it, which can cause nuisance trips, heating at connections and long-term corrosion at electrodes.

### Does lightning protection use the same earthing system as the power supply?

It should be bonded into the same overall earthing system rather than kept as an isolated electrode. An unbonded lightning earth can sit at a different potential to the power system earth during a strike, which is a safety risk and defeats much of the benefit of surge protection devices fitted on generators or switchboards.
