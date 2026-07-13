---
title: Joule-Thomson Effect
summary: Temperature change of a gas upon expansion through a valve, forming the basis for liquefaction.
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

# Joule-Thomson Effect

The Joule-Thomson (or Joule-Kelvin) effect describes the temperature change of a real gas or liquid when forced through a valve or porous plug while kept insulated so no heat is exchanged ($Q=0$).

## Thermodynamic Principle
The expansion through a throttle is an **isenthalpic** process, meaning Enthalpy ($H$) remains constant ($H_1 = H_2$).
- Work done: $W = P_1 V_1 - P_2 V_2$
- Internal Energy: $\Delta U = Q + W = 0 + (P_1 V_1 - P_2 V_2)$
- Therefore: $U_2 + P_2 V_2 = U_1 + P_1 V_1 \implies H_2 = H_1$

## Joule-Thomson Coefficient ($\mu_{JT}$)
The coefficient is defined as the rate of temperature change with respect to pressure at constant enthalpy:
$$\mu_{JT} = \left( \frac{\partial T}{\partial P} \right)_H = \frac{V}{C_p} (\alpha T - 1)$$
where $\alpha$ is the thermal expansion coefficient and $C_p$ is heat capacity.

Since expansion always involves a pressure drop ($\Delta P < 0$):
- If $\mu_{JT} > 0$, then $\Delta T < 0$ (The gas **cools**).
- If $\mu_{JT} < 0$, then $\Delta T > 0$ (The gas **heats** up).

## Inversion Temperature
The inversion temperature is where $\mu_{JT} = 0$ (occurring when $\alpha T = 1$). All real gases have an inversion curve on a P-T diagram with upper and lower inversion temperatures.
- To use the JT effect for cooling, the initial gas temperature must be below its maximum inversion temperature.
- Nitrogen and Oxygen have high inversion temperatures (e.g., N$_2$ is 621 K), so they cool upon expansion at room temperature.
- Hydrogen (204 K) and Helium (40 K) have low inversion temperatures. If expanded at room temperature, they heat up and can be dangerous (Hydrogen can explode). They must be pre-cooled before undergoing JT expansion.

## See Also
- [[gas-liquefaction]]
- [[refrigeration-cycles]]
