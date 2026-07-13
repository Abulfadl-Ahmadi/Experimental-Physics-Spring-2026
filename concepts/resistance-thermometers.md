---
title: Resistance Thermometers
summary: Temperature measurement using metals, semiconductors, thermistors, and diodes.
base_confidence: 0.9
lifecycle: draft
tier: core
sources:
  - "c:\\Users\\Mester\\Desktop\\semester 4\\Experimental Physics\\exam\\Chapter7-Processed.md"
provenance:
  extracted: 1.0
  inferred: 0.0
  ambiguous: 0.0
---

# Resistance Thermometers

Resistance thermometers infer temperature by measuring the electrical resistance of a material.

## Metal Resistance Thermometers
Metals (e.g., Platinum, Copper) typically increase in resistance with temperature due to increased electron scattering. 
Formula: $R = R_0(1 + aT + bT^2)$
- At low temperatures, impurity scattering (residual resistivity $\rho_i$) dominates, flattening the curve. A good low-temperature thermometer needs high purity to maintain a measurable $\partial\rho/\partial T$.

## Semiconductor Thermometers
- **Intrinsic Semiconductors**: Resistance increases rapidly as temperature drops because carrier concentration $n$ drops exponentially.
- **Doped Semiconductors**: Doping allows use at very low temperatures. They offer immense sensitivity (large $\partial\rho/\partial T$) but require individual calibration due to variations in doping concentrations.
- **Thermistors (NTC)**: Semiconductors with a Negative Temperature Coefficient. Resistance drops exponentially with heating. Very high accuracy (0.01°C).

## Carbon Resistors
Very cheap with good sensitivity at low temperatures. However, they suffer from poor repeatability and resistance drift over time.

## Diode Thermometers
Forward bias voltage across a p-n junction depends linearly on temperature above ~30K. Highly common in cryogenic applications (e.g., Silicon or GaAs diodes).

## See Also
- [[precision-resistance-measurement]]
