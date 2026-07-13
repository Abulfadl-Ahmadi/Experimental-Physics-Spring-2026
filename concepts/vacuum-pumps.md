---
title: Vacuum Pumps
summary: Classification and operating principles of various gas transfer and entrapment pumps used in vacuum technology.
base_confidence: 0.9
lifecycle: draft
tier: core
sources:
  - "c:\\Users\\Mester\\Desktop\\semester 4\\Experimental Physics\\exam\\Chapter6-Processed.md"
provenance:
  extracted: 1.0
  inferred: 0.0
  ambiguous: 0.0
---

# Vacuum Pumps

Pumps are used to evacuate chambers and create a [[vacuum]]. They fall into two main families: **Gas Transfer** (physically push molecules out) and **Entrapment** (capture and hold molecules).

## Mechanical Roughing Pumps
Operate from atmospheric pressure down to roughly $10^{-3}$ Torr. They usually act as primary or backing pumps.
- **Rotary Vane Pumps**: Use an oil seal between a sweeping vane and cylinder. Can suffer from oil backstreaming.
- **Roots Pumps**: Two figure-8 lobes rotate to move gas. Do not internally compress and must be backed by another pump.

## High-Vacuum Gas Transfer Pumps
Used to reach high and ultra-high vacuums.
- **Diffusion Pumps**: Use a heated fountain of heavy oil vapor to knock gas molecules downward. Requires cooling water, a cold trap (to prevent backstreaming), and a backing pump.
- **Turbomolecular Pumps**: Operate like a jet engine with high-speed rotating and fixed blades (up to 90,000 RPM) to transfer mechanical momentum to gas molecules. Requires a backing pump but is oil-free in the vacuum path.

## Entrapment Pumps (UHV)
Typically used for Ultra-High Vacuum environments. They trap gas inside the pump body.
- **Ion (Getter/Sputter) Pumps**: Ionize gas molecules with a strong electric field and bury them into Titanium cathode plates via sputtering. Do not use at atmospheric pressure (will burn out). 
- **Cryopumps**: Use extremely cold surfaces (down to 10-20K) to freeze and trap gases like $O_2, N_2, CO_2, H_2O$. Oil-free and excellent for semiconductor manufacturing, though struggling with Helium unless liquid Helium (3K) is used.

## Configuration & Sequencing
A typical system consists of a Roughing pump, a Secondary pump (Turbo/Diffusion), a cold trap, and valves.
**Critical Rule**: Never open the Gate valve connecting the chamber to the secondary pump until the chamber has been roughed down to operating pressure by the roughing pump.
