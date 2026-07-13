---
title: Gas Flow Regimes and Kinetic Theory
summary: Analysis of how gas molecules behave under varying pressure levels, governed by the Knudsen number and kinetic theory.
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

# Gas Flow Regimes and Kinetic Theory

The behavior of gases in a [[vacuum]] is determined by the frequency of molecular collisions, described by the **Knudsen Number ($Kn$)**.

## Knudsen Number
$$Kn = \frac{\lambda}{D}$$
Where $\lambda$ is the mean free path and $D$ is the dimension of the vacuum vessel.

- **Viscous (continuum) flow** ($Kn < 0.01$): Molecules collide with each other; behaves like a fluid.
- **Transitional flow** ($0.01 < Kn < 1$): Intermediate behavior.
- **Free Molecular flow** ($Kn > 1$): Molecules bounce off the walls of the chamber more frequently than they collide with each other.

## Kinetic Theory Properties

### Molecular Impact Rate
The rate at which gas molecules hit the walls of a chamber (determining gas load or contamination):
$$z = \frac{P}{\sqrt{2\pi m k T}}$$

### Monolayer Formation Time
The time required for a single layer of molecules to coat a completely clean surface.
Even at $10^{-5}$ Pa, it takes only ~12.8 seconds for a monolayer of Hydrogen to form, demonstrating why UHV requires extreme cleanliness.

### Mean Free Path ($\lambda$)
The distance a molecule travels before hitting another.
- At 1 bar: ~70 nm
- At $10^{-7}$ Pa: ~64 km
- At $10^{-10}$ Pa (UHV): ~64,000 km (bounces purely off walls).

### Velocity Distribution
Described by the Maxwell-Boltzmann distribution. Baking vacuum chambers increases the kinetic energy of adsorbed molecules, pushing them into the gas phase to be pumped away.

## Pumping Speed & Conductance
- **Pumping speed ($S$)**: Volumetric flow rate ($dV/dt$) in L/s.
- **Throughput ($Q$)**: The actual quantity/mass of gas moving per second ($Q = P \cdot S$). Throughput remains constant in a pumping system.
- **Conductance ($C$)**: Dictates the flow capability of a pipe (analogous to electrical conductance).
  - Effective pumping speed is limited by conductance: $\frac{1}{S_{eff}} = \frac{1}{C} + \frac{1}{S_{nom}}$

## Gas Loads
The ultimate pressure limit is dictated by the total gas load divided by the pumping speed ($P_{ultimate} = \frac{Q_{out}}{S}$). 
Gas sources include permeation, real leaks, desorption (outgassing), virtual leaks, back-streaming, and evaporation.
