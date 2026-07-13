---
title: Precision Resistance Measurement
summary: Circuit configurations to eliminate lead resistance errors when measuring precision resistance thermometers.
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

# Precision Resistance Measurement

When measuring the resistance of sensors (like [[resistance-thermometers]]), the resistance of the lead wires can introduce significant errors. Specialized circuits are used to compensate for this.

## Four-Probe Method
Eliminates lead resistance errors entirely. 
- Two outer probes supply a known current ($I$).
- Two inner probes measure the voltage drop ($V$).
- Because the voltage measurement path draws virtually zero current (due to the high input impedance of the voltmeter), the resistance of those specific leads does not affect the voltage reading.
- Resistivity formula: $\rho_0 = (V / I) \cdot 2\pi S$ (where $S$ is probe spacing).

## Wheatstone Bridge
Suitable for resistances from 1 $\Omega$ to 10 $M\Omega$. 
At balance (galvanometer current is zero), the unknown resistance $R_x$ is found via:
$$R_x = R_3 \cdot \frac{R_2}{R_1}$$

**Error sources** in Wheatstone bridges include:
- Resistance changes due to self-heating ($I^2R$).
- Thermal EMFs or contact potentials.
- Lead connection errors.

## Lead Resistance Compensation Methods
When using bridges, various three-lead or four-lead arrangements (e.g., Siemens's three-lead, Callender four-lead) are used so that lead resistances either cancel out or are added equally to both the unknown and the reference branches.
