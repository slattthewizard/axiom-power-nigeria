---
meta_title: "Pump Cavitation: Causes, NPSH and Fixes for Nigerian Plants"
meta_description: "Pump cavitation explained for plant engineers in Nigeria: NPSHa vs NPSHr, suction-side causes, warning sounds, impeller damage and practical fixes."
primary_keyword: "pump cavitation"
secondary_keywords: "cavitation in pumps, npsh, cavitation causes, cavitation damage"
---

# Pump Cavitation: Causes, Warning Signs and Fixes for Industrial Sites

A centrifugal pump that suddenly sounds like it is pumping gravel, loses pressure at the discharge gauge, and runs hotter than usual is very often suffering pump cavitation rather than a mechanical fault on its own. Cavitation is a suction-side problem that shows up as a noise and vibration complaint, which is why maintenance teams sometimes chase the wrong component before someone checks the suction conditions.

This article sets out what cavitation actually is, how to tell it apart from other pump problems, the site conditions in Nigeria that bring it on, and the checks and fixes that reduce or remove it. It assumes a standard centrifugal pump handling water, effluent or a similar liquid, of the kind found on cooling towers, firewater rings, boiler feed, effluent transfer and process water duty across factories, oil and gas facilities, hospitals and IPPs.

## What Cavitation Is, in Plain Terms

Inside a centrifugal pump, liquid pressure drops as it accelerates into the eye of the impeller. If that local pressure falls below the liquid's vapour pressure at the temperature it is running at, small vapour bubbles form. A moment later, as the liquid moves into the higher-pressure zone further along the impeller vanes, those bubbles collapse violently. Each collapse sends out a tiny, high-energy shock. Millions of these collapses happening every second are what produce the characteristic noise, the vibration, and, over time, the pitting on the impeller and casing.

Cavitation is fundamentally a shortage of usable pressure at the pump suction, not a fault that starts inside the pump itself. That distinction matters for diagnosis: replacing an impeller or bearing on a cavitating pump without fixing the suction side buys very little time.

## NPSHa vs NPSHr: The Numbers That Decide It

Two figures govern whether a pump will cavitate.

**NPSHr (Net Positive Suction Head required)** is a property of the pump itself, set by its design and stated on the manufacturer's performance curve for a given flow rate. It rises as flow rate rises, which is one reason a pump that runs quietly at reduced flow can start cavitating once demand increases.

**NPSHa (Net Positive Suction Head available)** is a property of the installation: the suction source level, the pressure above the liquid, the vapour pressure of the liquid at its operating temperature, and the friction losses in the suction pipework, fittings and strainer between the source and the pump.

The pump avoids cavitation only where NPSHa stays comfortably above NPSHr across the flow range the pump actually runs at, not just at its rated duty point. Manufacturer datasheets for a typical centrifugal pump show NPSHr climbing steadily as flow increases past the best efficiency point, so a pump sized generously at design flow can still cavitate if it is later run wide open or against a lower head than intended. The OEM curve for the specific pump model and impeller trim governs; NPSHa and NPSHr should always be checked against that curve rather than assumed from a similar pump elsewhere on site.

## Suction-Side Causes Common on Nigerian Sites

Most cavitation traces back to one or more of the following on the suction side.

- **Suction lift that is too high.** A pump drawing from a sump, borehole or low tank below pump centreline has less NPSHa available than one fed by gravity flow. Long suction runs, tight bends and undersized suction pipe all add friction losses that eat into that margin further.
- **Hot liquid.** As liquid temperature rises, its vapour pressure rises too, which reduces the NPSH margin at the same suction arrangement. Boiler feed pumps, hot condensate pumps and pumps drawing from a warm cooling tower basin are more exposed than pumps on cold raw water, and ambient heat on site pushes liquid temperatures up further than a cooler climate would.
- **Clogged or undersized strainers.** A partially blocked suction strainer or foot valve adds friction loss that was never in the original design calculation. This is one of the most common site causes because it develops gradually and is easy to miss between inspections, particularly where raw water carries silt or where a sump collects debris.
- **Undersized or poorly laid out suction pipework.** Suction pipe a size smaller than the pump inlet, unsupported horizontal runs with air pockets, or an elbow fitted directly onto the pump suction flange, all reduce NPSHa below what the original pipe sizing calculation assumed.
- **Low tank or sump level.** Running a suction tank down close to empty, or a vortex forming as level drops, lets air enter the suction line and produces symptoms very similar to true cavitation, sometimes called air entrainment rather than vapour cavitation, but the fix is usually the same: restore adequate submergence and suction conditions.
- **Running off the curve.** A pump throttled hard on discharge, or run at unusually high flow because a downstream valve is left wide open, moves away from its best efficiency point and can push NPSHr above what the installation can supply.

Take a hypothetical 200 cubic metre per hour transfer pump drawing from an open sump: if the strainer fouls by half over a few weeks of operation, the added friction loss can be enough on its own to tip a previously adequate NPSH margin into cavitation, with no change to the pump, motor or piping.

## Sound, Vibration and Performance Signs

Cavitation gives warning before it causes serious damage, if the signs are read correctly.

- A rattling, crackling or "gravel" noise from the pump casing, most noticeable near the suction side, that changes with flow rate.
- Vibration readings that rise at the same time as the noise, often broadband rather than a single clean frequency.
- Discharge pressure that fluctuates or sags below the expected point on the pump curve for the current flow.
- Flow that will not increase further no matter how far the discharge valve is opened.
- Higher motor current draw than expected for the apparent duty, as the pump works inefficiently against the vapour pockets.
- Warmer than normal bearing housings on prolonged cavitation, from the extra vibration loading.

None of these signs is conclusive on its own; a worn bearing, misalignment or a loose foundation bolt can produce similar noise and vibration. That is why the suction-side checks below matter as much as the symptom itself.

| Symptom at the pump | Likely suction-side cause | Check to confirm |
|---|---|---|
| Gravel/crackling noise near suction, worse at high flow | Insufficient NPSHa for the current flow rate | Compare NPSHa calculation against NPSHr on the pump curve at that flow |
| Noise and vibration that ease when discharge valve is throttled back | Running the pump beyond its efficient flow range | Read flow and compare to the pump's best efficiency point |
| Sudden onset after weeks of quiet running | Strainer or foot valve fouling | Inspect and clean strainer, check differential pressure across it |
| Noise that varies with tank or sump level | Low submergence, vortexing at suction inlet | Check level against minimum submergence for the suction bell or pipe |
| Noise worse when liquid is hotter (e.g. after a process upset) | Rising vapour pressure reducing NPSH margin | Check liquid temperature against the NPSH calculation basis |

## What Cavitation Damage Looks Like

Left running, cavitation removes material from the impeller vanes and, in severe cases, the volute casing near the impeller eye. The pitting has a rough, sponge-like or honeycombed appearance, usually concentrated on the low-pressure (suction) side of the vanes rather than spread evenly. Left long enough, it thins the vanes to the point of reduced efficiency, imbalance, or vane fracture.

The vibration that comes with cavitation also shortens bearing and mechanical seal life well before the impeller itself fails outright. A seal designed for smooth hydraulic conditions can start leaking under sustained cavitation-induced vibration long before anyone notices impeller wear, which is often the first sign that gets a cavitating pump pulled for inspection. On some duties, cavitation erosion can progress to a through-wall hole in the casing wall in a matter of months of continuous running, depending on liquid, pressure and how severe the vapour collapse is.

## Fixes and Prevention

The correct fix follows from the cause, not from a generic parts swap.

- Rework the suction pipe layout: larger diameter, fewer fittings close to the pump, no high points that trap air, and a straight run into the suction flange where the pump manufacturer's installation drawing calls for one.
- Clean or resize the suction strainer and set a routine to check differential pressure across it rather than waiting for symptoms.
- Raise the effective suction head where possible: raise the source tank, lower the pump, or reduce suction lift.
- Reduce liquid temperature at the pump inlet where the process allows, or select a pump with a lower NPSHr for hot duty.
- Match the pump's operating point closer to its best efficiency point through correct valve settings, trimmed impeller, or a variable-speed drive rather than running permanently throttled or wide open.
- Where the installation genuinely cannot supply enough NPSHa, specify a pump with a lower NPSHr for the same duty, or add a small booster pump ahead of the main pump.

Any of these changes to piping, pump internals or drive arrangements should be scoped from a proper site survey and the specific pump's performance curve, not from symptoms alone. Work on suction piping, impeller removal or seal replacement on rotating equipment should only be carried out by qualified personnel under lockout/tagout and a permit to work, with the pump isolated and depressurised before any component is opened. A structured look at the pump, its suction arrangement and its duty point against a proper cavitation assessment, alongside the rest of the plant's rotating equipment, is covered under [rotating equipment and compressor services](/rotating-equipment-services-nigeria/); if cavitation is a recurring problem on a critical pump, [book a plant assessment](/#contact) rather than replacing parts repeatedly on the same fault.

## Frequently Asked Questions

### How can I tell cavitation apart from a worn bearing?

Cavitation noise tracks with flow and suction conditions: it changes when you throttle the discharge valve or when tank level drops, while bearing noise is usually steady regardless of flow. A vibration reading that is broadband and concentrated near the suction side, alongside a discharge pressure that will not hold at the expected point on the pump curve, points to cavitation rather than a bearing fault, though a full check should confirm which is present.

### Does cavitation always damage the pump?

Not immediately. Light, intermittent cavitation mainly shows up as noise and a small efficiency loss, and stops causing wear once the suction condition is corrected. Sustained, heavy cavitation is what pits impeller vanes and casings and shortens seal and bearing life, so the risk depends on how severe and how long-running the condition is, not on whether cavitation occurred at all.

### Can a strainer alone cause cavitation?

Yes. A fouled or undersized suction strainer adds friction loss that was never accounted for in the original NPSHa calculation, and this is one of the more common causes found on site inspections. Restoring the strainer to its clean condition, or resizing it, often resolves cavitation that appeared without any change to the pump or piping.

### Is air entrainment the same thing as cavitation?

They produce similar noise and vibration but are different mechanisms. True cavitation is vapour bubble formation and collapse from a local pressure drop below the liquid's vapour pressure; air entrainment is air being drawn into the suction line, often from a low tank level or a vortex at the suction inlet. Both are corrected by improving suction conditions, so the practical checks overlap even though the underlying cause differs.

### What NPSH margin should a pump be designed with?

The margin needed depends on the specific pump, its impeller design and the service, so the pump manufacturer's curve and application guidance for that model should set the figure rather than a fixed rule of thumb applied across every pump on site. A pump running consistently close to its stated NPSHr, with little margin against real site conditions such as strainer fouling or seasonal temperature rise, is the one most likely to cavitate first.
