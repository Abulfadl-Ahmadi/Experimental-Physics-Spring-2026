---
title: Optical and Radiation Thermometry
summary: Non-contact temperature measurement using blackbody radiation and pyrometers.
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

# Optical and Radiation Thermometry

These methods measure temperature without physical contact by analyzing emitted thermal radiation.

## Blackbody Radiation Theory
- **Planck's Law**: Describes the energy density of emitted radiation across frequencies. The peak emission frequency shifts higher as temperature increases.
- **Stefan-Boltzmann Law**: Total radiated energy is proportional to the fourth power of temperature ($q/A = \epsilon \sigma T^4$), where $\epsilon$ is the emissivity.

## Optical Pyrometer
Matches the brightness of a hot object with a calibrated internal tungsten filament. The observer adjusts the filament current until the filament "disappears" against the background of the object, indicating matched temperatures.

## Emissivity Corrections
Real objects are not perfect blackbodies; their emissivity ($\epsilon$) is less than 1.
Failing to account for true emissivity causes temperature under-reporting.
For example, if measuring metal with actual $\epsilon=0.75$ but assuming $\epsilon=0.82$, an apparent reading of 1050°C (1323K) requires correction:
$$T_{real} = 1323 \cdot (0.82 / 0.75)^{1/4} = 1352 K$$
A relatively large error in emissivity yields a proportionally smaller error in absolute temperature due to the fourth-root dependence.
