---
title: Thermocouples
summary: Temperature measurement based on the Seebeck effect using dissimilar metal junctions.
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

# Thermocouples

Thermocouples operate on the **Seebeck Effect**: When a material experiences a temperature gradient, electron distribution shifts, creating a potential difference ($\Delta V = S(T) \cdot \Delta T$). 
$S(T)$ is the Seebeck coefficient (thermoelectric power).

## Operating Principle
A thermocouple joins two dissimilar metals. The net voltage output depends on the temperature difference between the measurement (hot) junction and a reference (cold) junction, as well as the difference in Seebeck coefficients:
$$\Delta V_T = [S_1(T) - S_2(T)] \delta T$$

## Reference Junctions
To obtain absolute temperatures, the reference junction must be kept at a known temperature (traditionally an ice-water bath at 0°C). 

## Types of Thermocouples
Different metal pairs provide optimal sensitivity in different ranges:
- **Type K**: Chromel/Alumel (-200 to 1250°C)
- **Type J**: Iron/Constantan (0 to 750°C)
- **Type T**: Copper/Constantan (excellent for cryogenics down to -200°C)
- **Type S/R**: Platinum/Rhodium alloys (high temperatures up to 1450°C)

## Desired Characteristics
A good thermocouple pair needs stability at service temperatures (no melting/oxidation) and a large difference in Seebeck coefficients for high sensitivity.
