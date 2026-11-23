---
meta_title: "Black Smoke from Generator: Causes by Colour and Checks"
meta_description: "Black, white or blue smoke from a diesel generator points to different faults. Learn what each colour means, what to check first and when to shut down."
primary_keyword: "black smoke from generator"
secondary_keywords: "generator white smoke, blue smoke diesel generator, generator exhaust smoke causes, diesel generator smoke"
---

# Black Smoke from Generator: What Each Exhaust Colour Is Telling You

A diesel engine that's running properly makes an almost clear exhaust, maybe a faint haze at a cold start and a little grey when the load steps up. Anything heavier than that is the engine telling you something, and the colour narrows the list of suspects faster than any other single clue you can get without opening a panel.

Black, white and blue smoke are three different problems. Black means fuel that isn't burning completely. White means unburnt fuel vapour or water in the cylinders. Blue means lubricating oil is getting into the combustion chamber.

This guide covers the likely causes of each colour, what to check first, and where the line sits between "book it for the next service" and "stop it now".

## Read the smoke before you touch anything

Note whether the smoke appears at start-up, on load acceptance, under steady load or when the load drops. Check the control panel for load, coolant temperature and oil pressure, and read the controller event log before you reset anything. A set that has run clean for months and now smokes usually has a single failed component. Gradual change over hundreds of hours usually means wear.

## Black smoke: fuel without enough air

Black smoke is soot. The engine is injecting more fuel than the air in the cylinder can burn, or the fuel is arriving at the wrong moment and burning badly. It's the colour most people search for first, and honestly, the cause is usually either too much load or too little air.

The common causes, roughly in order of how often they turn out to be the answer:

- Overload. The set is carrying more than its rating, or a large motor start has pushed it past what it can deliver. Black puffs on load acceptance that clear after a few seconds are often just a big step load and not a fault. Sustained black smoke at a high load reading is a sizing or loading problem.
- Restricted intake air. A choked air filter, a collapsed intake hose, or a blocked room louvre starves the engine. In dusty seasons this happens faster than the service schedule assumes.
- Turbocharger problems. A turbo that isn't delivering boost leaves the engine short of air at the same fuel setting. Low boost, a whistling or grinding noise and oil at the compressor outlet all point this way. There's more on this in our guide to [turbocharger failure in generators](/blog/turbocharger-failure-generator/).
- Injector or pump faults. Worn or leaking injectors, a sticking nozzle or an out-of-calibration injection pump spray fuel badly or too much of it. This one is more common on older sets and on engines that have run on poor fuel. See the notes on [injector pump problems](/blog/injector-pump-problems/).
- Wrong injection timing. After a pump or timing gear job, timing that's retarded makes fuel burn late and smoke black or grey-black.

## White smoke: cold start, water or unburnt fuel

White smoke needs more care in interpretation, because it ranges from harmless to serious.

A short burst of white smoke on a cold start is normal on many diesels: unburnt fuel vapour and condensed water that thins out as the engine warms. If it persists once warm, treat it as a fault.

Persistent white smoke has several possible causes:

- Coolant entering the cylinders. A failed head gasket, a cracked head or a damaged liner lets coolant into the combustion chamber, where it flashes to steam. The smoke is thick, has a sweet smell and tends to go with a falling coolant level, bubbles in the radiator header and sometimes milky oil on the dipstick. This is the case that needs a shutdown. Our article on [head gasket failure in generators](/blog/head-gasket-failure-generator/) covers the confirmation tests.
- Water in the fuel. Water in the tank or the filters causes misfire, rough running and white smoke. In plants where diesel is delivered by tanker and stored for long periods, this is more common than most people expect.
- Low compression. Worn rings or poorly seated valves reduce the temperature at the end of compression, so fuel doesn't ignite properly and leaves as white vapour.
- One cylinder misfiring. If the smoke comes with a rough note and uneven exhaust temperature, a dead injector on one cylinder is the likely cause.

## Blue smoke: engine oil in the combustion chamber

Blue smoke, sometimes a bluish grey, is burning lubricating oil. It has a distinctive acrid smell, quite unlike the sharp smell of raw diesel. The oil is getting past something it shouldn't:

- Worn piston rings or cylinder liners, which let oil climb into the chamber. This is usually accompanied by rising oil consumption, a high crankcase breather flow and lower compression.
- Worn valve stem seals or guides, which let oil run down the valve stems. A classic sign is a puff of blue smoke on start-up after the engine has stood overnight, clearing once it runs.
- Turbocharger oil seals. A worn turbo shaft seal passes oil into the intake or exhaust side. If the smoke comes with oil in the intercooler pipes, look at the turbo first.
- Wet stacking from light load. This is the one that catches plants out. A set that runs for long periods at low load never gets hot enough for the rings to seal and the fuel to burn completely. Unburnt fuel and oil collect in the exhaust and show as blue-grey smoke, sometimes with oily black droplets at the exhaust outlet. We cover this in detail in the article on [diesel generator wet stacking](/blog/diesel-generator-wet-stacking/).

Wet stacking is a loading problem, not a mechanical defect, at least to begin with. Run a set lightly for months and it will start to smoke blue-grey and leave glazed bores and carbon in the exhaust. The fix is to bring the load up to a sensible level, not to replace parts. As a rough guide for context, a healthy diesel set burns around 0.27 to 0.30 litres per kWh at 75 to 100 percent load, but closer to 0.38 at 30 percent load. If your fuel consumption per kWh has drifted toward the higher figure and the set smokes blue-grey, light loading is the first thing to question.

## Colour, likely causes and first checks

This table puts the above in one place. Use it as a starting point, not a diagnosis. Plenty of faults overlap.

| Smoke colour | Most likely causes | First checks | Shut down when |
|---|---|---|---|
| Black | Overload, choked air filter, turbo underperforming, injector or pump fault, late timing, blocked exhaust | Load reading, air filter indicator, intake ducting, boost pressure, exhaust back pressure | Sustained thick black with rising exhaust temperature, loss of power or turbo noise |
| White (brief, at start) | Normal cold start, weak cold-start aid | Time to clear, coolant temperature, glow plug or heater operation | Does not clear when warm |
| White (persistent) | Coolant in cylinders, water in fuel, low compression, one cylinder misfiring | Coolant level and bubbles, oil colour, fuel filter bowl drain, exhaust temperature by cylinder | Coolant loss, milky oil, overheating or rough running |
| Blue | Worn rings or liners, valve stem seals, turbo oil seals, overfilled sump, blocked breather | Oil level and consumption, breather, turbo pipework for oil, start-up versus steady smoke | Oil level dropping fast, oil pressure falling, or runaway speed |
| Blue-grey with oily deposits | Wet stacking from long light-load running | Load history, fuel use per kWh, exhaust outlet for oily residue | Rarely urgent, but correct the loading soon |

## What to check first, in order

Read the controller first: load, coolant temperature, oil pressure and logged alarms. A set at full rated load on a hot day with a dirty filter will smoke black with no real fault. Then check air (filter restriction indicator and intake path), then liquids (coolant level, oil level and condition, where milky oil or rising coolant are red flags), then fuel. Drain a small sample from the water trap or filter bowl; water, sediment or cloudiness points straight to contaminated diesel. Finally, listen for a turbo whine, a misfire pattern or a knock.

Any hands-on work beyond observation, such as removing filters, opening the exhaust or checking injectors, needs the set isolated and locked out, the starting system disabled, and a permit to work in place. Exhaust components stay hot long after shutdown, and an engine that appears stopped can still be started by an AMF panel or a remote signal.

## When to shut the set down

Stop the engine, following your site procedure, for thick white smoke with coolant loss or overheating, because coolant in the cylinders can hydraulically lock an engine and bend a connecting rod. Stop it if blue smoke comes with falling oil pressure, if the engine speeds up uncontrolled, if you hear metallic knocking, or if black smoke comes with rapid power loss and rising exhaust temperature.

If it's a steady thin black or blue haze and everything else reads normal, you can usually run at reduced load until the next planned window, but don't leave it indefinitely. A set left smoking for months turns a cheap fix into a rebuild.

## Getting a proper diagnosis

Colour gets you to a short list, not the answer. Confirming the cause usually takes measured boost pressure, exhaust temperature by cylinder, a compression or leak-down test, an injector test, and fuel, oil and coolant samples. Those are jobs for trained people with the right tools. If smoke keeps recurring, look at the pattern: a certain load profile, a fuel delivery, a season or a maintenance gap often tells you more than the engine does.

Smoke from your generator that you can't explain, or a set that keeps coming back with the same fault? You can request a technical proposal through our [contact page](/#contact) and our engineers will assess the set on site.

## Frequently Asked Questions

### Is a little black smoke at start-up normal on a diesel generator?

Yes, a brief puff of black or dark grey smoke when the set picks up a large load, or for a few seconds after start-up, is common and usually harmless. It's a concern when it continues under steady load, gets worse over weeks or comes with a loss of power.

### Why is my generator producing white smoke after it's warmed up?

Persistent white smoke on a warm engine suggests coolant or water entering the cylinders, water in the fuel, low compression or a misfiring cylinder. Check the coolant level, the oil colour and the fuel water trap. If you see coolant loss or milky oil, shut the set down.

### Does blue smoke always mean the engine needs a rebuild?

No. Blue smoke can come from an overfilled sump, a blocked breather, worn valve stem seals or a leaking turbo seal, all of which cost far less than a rebuild. Long periods of light load can also cause blue-grey smoke through wet stacking, which is usually cured by loading the set properly and cleaning the exhaust system.

### Can I keep running a generator that's smoking?

It depends on the colour and the other readings. Thin smoke with normal pressures and temperatures can usually run at reduced load until a planned stop. Thick white smoke with coolant loss, blue smoke with falling oil pressure, or black smoke with power loss and rising exhaust temperature means stop the set and investigate.

### How do I stop my generator smoking from light-load running?

Raise the average load toward the range where the engine runs hot and clean, ideally above roughly 60 to 70 percent of rating for prime duty. Where site demand is low, consider a smaller set, load sharing across multiple sets, or a planned load bank run to burn off deposits.
