---
title: Pressure Gauges
summary: Operating principles and application ranges of vacuum pressure measurement tools.
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

# Pressure Gauges

No single gauge can measure the entire pressure range from atmosphere to Ultra-High [[Vacuum]]. Different physical principles apply to different regimes.

## Mechanical & Fluid Gauges (Atmosphere to Rough Vacuum)
- **U-Tube Manometer**: Measures the height difference of a fluid column. Pressure difference depends directly on density difference between manometer fluid and the system gas.
- **Well-Type Manometer**: Uses a large reservoir to simplify calculations ($P_1 - P_2 = \rho \cdot g \cdot h$).
- **McLeod Gauge**: An absolute gauge that compresses a known volume of gas into a capillary. Historically the gold standard for very low pressures before electronic sensors.

## Electronic Gauges (High to Ultra-High Vacuum)
- **Pirani Gauge**: Uses a heated filament. As pressure drops, fewer gas molecules collide with the wire, reducing heat loss. The wire gets hotter, altering its resistance. Usually combined with a sealed reference gauge for temperature compensation. Covers down to $\sim 10^{-4}$ Pa.
- **Ionization Gauge**: The standard for Ultra-High Vacuum ($\sim 10^{-2}$ to $10^{-10}$ Pa). It ionizes gas molecules using a hot filament (or radioactive source like the Alphatron gauge) and measures the resulting ion current. 
  - **Warning**: Must NEVER be turned on at atmospheric pressure, or the hot filament will immediately burn out.

## See Also
- [[vacuum-pumps]]
