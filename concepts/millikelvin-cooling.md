---
title: Millikelvin Cooling
summary: Methods to achieve temperatures below 4 K, including pumped helium, dilution refrigerators, and adiabatic demagnetization.
base_confidence: 0.9
lifecycle: draft
tier: core
sources:
  - "c:\\Users\\Mester\\Desktop\\semester 4\\Experimental Physics\\exam\\_raw\\Chapter8-Processed.md"
  - "c:\\Users\\Mester\\Desktop\\semester 4\\Experimental Physics\\exam\\_raw\\Chapter8-Processed2.md"
provenance:
  extracted: 1.0
  inferred: 0.0
  ambiguous: 0.0
---

# Millikelvin Cooling

Standard liquid helium (Helium-4) boils at 4.2 K. Special techniques are required to reach the millikelvin range.

## Evaporative Cooling (Pumped Helium)
By vigorously pumping the vapor away from a bath of liquid helium, the pressure drops, which lowers the boiling point (following the Clausius-Clapeyron relation).
- Pumping on $^4$He can reach about **1.0 K**.
- Pumping on the much rarer isotope $^3$He (which has a higher vapor pressure at low temperatures) can reach about **0.25 K (250 mK)**.

## Dilution Refrigeration ($^3$He/$^4$He)
The only continuous cooling method to reach down to **~10-20 mK**.
**Principle**: 
Below ~0.8 K, a mixture of $^3$He and $^4$He spontaneously separates into two phases:
1. A concentrated (lighter) phase of almost pure $^3$He.
2. A dilute (heavier) phase of $^3$He dissolved in superfluid $^4$He.

Cooling occurs in the **Mixing Chamber** when $^3$He atoms are forced across the phase boundary from the concentrated phase into the dilute phase. This "evaporation" of $^3$He into the $^4$He background is an endothermic process that absorbs heat from the sample. The system continuously pumps $^3$He out of a "Still", purifies it, and returns it to the mixing chamber to sustain the cycle.

## Magnetic Cooling (Adiabatic Demagnetization)
Used to reach microkelvin temperatures.
1. **Isothermal Magnetization**: A strong magnetic field aligns the magnetic dipoles of a paramagnetic salt, decreasing its magnetic entropy. The heat generated is removed by a thermal link to a precooler (like a dilution fridge).
2. **Adiabatic Demagnetization**: The thermal link is broken, isolating the sample. The magnetic field is slowly reduced to zero. The dipoles tend to randomize, absorbing thermal energy from the crystal lattice, causing the temperature of the material to drop precipitously.
