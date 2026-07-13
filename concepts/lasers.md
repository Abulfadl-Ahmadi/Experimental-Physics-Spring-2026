---
title: Lasers
summary: Principles of stimulated emission, population inversion, and common types of lasers.
base_confidence: 0.9
lifecycle: draft
tier: core
sources:
  - "c:\\Users\\Mester\\Desktop\\semester 4\\Experimental Physics\\exam\\Chapter9-Processed.md"
provenance:
  extracted: 1.0
  inferred: 0.0
  ambiguous: 0.0
---

# Lasers

**LASER** stands for Light Amplification by Stimulated Emission of Radiation. Laser light is highly coherent (in-phase), intense, and monochromatic.

## Working Principle
Lasers rely on **Population Inversion**: a state where more atoms are in an excited energy state ($E_2$) than in the lower state ($E_1$). 
When a photon of energy $h\nu = E_2 - E_1$ interacts with an excited atom, it triggers **stimulated emission**, causing the atom to release a second identical photon in phase with the first.
This process occurs in an **Optical Resonator** (a cavity between a 100% reflective mirror and a partially reflective mirror), which bounces the light back and forth to rapidly amplify the beam. The active medium is energized by a "pump" (optical, electrical, RF, etc.).

## Common Laser Types

### Helium-Neon (He-Ne) Gas Laser
- Emits continuous wave (CW) red light at **632.8 nm**.
- Contains He and Ne (approx 10:1 ratio) at low pressure (1-10 torr).
- **Mechanism**: Electrical discharge pumps Helium to an excited state. Through collisions, Helium transfers this energy to Neon (which has matching energy levels). Neon then undergoes stimulated emission to produce the laser beam.

### Carbon Dioxide ($CO_2$) Gas Laser
- A mixture of $N_2$ and $CO_2$. Nitrogen is electrically pumped and transfers energy to the *vibrational* states of $CO_2$.
- Emits intense infrared radiation (**10.6 $\mu$m** and 9.6 $\mu$m).
- Used extensively in industrial cutting/engraving and medical surgery (tissue cutting).

### Dye Lasers
- Use an organic dye (e.g., Rhodamine 6G) in liquid solution as the gain medium.
- Very broad emission bandwidth allows them to be **tunable** across a wide range of wavelengths (50-100 nm tuning range). They exhibit a Stokes shift (absorbing at shorter wavelengths, emitting at longer ones).

### Solid-State Lasers
- Include semiconductor diode lasers (e.g., GaAs emitting at 868 nm) and crystal lasers like Nd:YAG (emitting near 1064 nm) or Ruby.

## Monochromaticity
A laser beam is not perfectly monochromatic. The output wavelength is dictated by the resonant cavity modes ($L = n \lambda / 2$). The laser's spectral width can contain several of these extremely narrow, closely spaced modes (e.g., spaced by 0.002 nm) within the natural atomic transition linewidth.
