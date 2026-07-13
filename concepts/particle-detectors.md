---
title: Particle Detection and Spectroscopy
summary: Methods for separating and detecting high-energy particles, including the Geiger-Muller tube.
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

# Particle Detection and Spectroscopy

Detecting and separating particles based on energy/wavelength requires specialized tools depending on the particle type.

## Optical Spectroscopy Principles
To identify photons or wave-like particles based on wavelength, a spectrometer uses:
1. **Source**: The light or particle source.
2. **Collimator**: To create parallel rays.
3. **Wavelength Separator**: A Prism (relies on refraction) or a Diffraction Grating (relies on wave diffraction/interference geometry) to spread out the spectrum.
4. **Detector**: To measure the intensity of the isolated wavelength.

## Geiger-Muller Detector
A robust gas-filled detector used to count ionizing radiation (Alpha, Beta, Gamma, X-rays).
**Structure**: A cylindrical capacitor (metal wall as cathode, central wire as anode) filled with an inert gas.
**Operation**:
- An incoming particle ionizes a gas atom, creating an electron and a positive ion.
- A high voltage across the cylinder causes the electron to accelerate toward the central wire so rapidly that it ionizes further gas atoms on the way (a Townsend avalanche).
- This creates a massive, easily detectable electrical pulse.
- **Geiger-Muller Plateau Region**: In this specific operating voltage range, the detector operates in "saturation". The size of the output pulse is independent of the initial energy or type of the incoming particle; it only registers that a detection event occurred (it counts particles, but does not measure their energy).

## Key Parameters of Detectors
When selecting any detector, experimentalists evaluate:
1. **Sensitivity**: Signal-to-noise ratio and detection limits.
2. **Response Speed**: Ranges from nanoseconds (PMTs) to minutes (thermal).
3. **Response Range**: Applicable wavelength or energy range.
4. **Selectivity**: Ability to distinguish the target signal from background noise.
5. **Cost**: Fabrication and lifespan.
6. **Environmental Safety**.
