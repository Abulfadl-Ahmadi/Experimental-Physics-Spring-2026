---
title: Photon Detectors
summary: Devices that convert optical signals into electrical signals, from simple photoresistors to sensitive photomultipliers.
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

# Photon Detectors

Photon detectors (O/E Converters) generate an electrical signal when exposed to light. 
Key requirements for a good detector include wavelength selectivity (high responsivity at the desired wavelength), fast response time (high bandwidth), low noise, and temperature stability.

## Photoelectric Detectors
Rely on the external photoelectric effect. If incoming photons have energy greater than the material's work function ($h\nu > \Phi$), electrons are ejected from the surface, generating a current in a vacuum tube.

## Photoresistive Detectors (LDR)
Light Dependent Resistors (LDRs) are made of semiconductors. When photons with energy greater than the bandgap ($h\nu > E_g$) are absorbed, they excite electrons from the valence band to the conduction band. 
This creates electron-hole pairs ($\Delta n = \Delta p$), increasing the overall charge carrier concentration and decreasing the resistance. The change in conductivity is proportional to the light intensity.
*Applications*: Ambient light sensors for automated room lighting, simple presence detection.

## Photodiodes
Semiconductor P-N or PIN junctions designed to absorb light. When illuminated by photons of appropriate energy, electron-hole pairs are created in the depletion region. Under reverse bias voltage, these carriers are swept apart by the electric field, drastically increasing the reverse (dark) current in proportion to the light intensity.
*Advantages*: High speed, linear response, highly compact.

## Thermal Detectors
Used primarily in the Infrared region. They detect radiation by measuring a change in temperature (and a corresponding change in resistance) caused by absorbed heat.
*Characteristics*: Slower response time compared to photoelectric detectors. Used in thermal imaging cameras and fever-screening sensors.

## Photomultiplier Tubes (PMT)
Extremely sensitive detectors capable of measuring single photons (used in fluorescence spectroscopy, nuclear physics, and medical imaging).
- A photon strikes a **Photocathode**, ejecting a primary electron via the photoelectric effect.
- The electron is accelerated by a high voltage (via a resistive voltage divider circuit) towards a series of electrodes called **Dynodes**.
- Each dynode emits multiple secondary electrons when struck by one electron ($\text{Gain} = \delta^n$).
- The avalanche of electrons is collected at the Anode, producing a massive electrical pulse (amplification up to $10^7$ times) for a single initial photon.
