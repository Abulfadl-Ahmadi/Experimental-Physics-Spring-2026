# Thermometry (Temperature Measurement) - Content by Topic

## 1. Ideal Thermometer Requirements

**Required Characteristics:**
1. Sufficient accuracy
2. Temporal stability and tolerance to environmental conditions (very hot, cold, high radiation, high/low pressure, air flow, etc.)
3. Competitive and reasonable price
4. Wide and expected working range
5. Easy and cheap calibration capability
6. Small size and appropriate shape to achieve thermal equilibrium with the intended environment (sufficient means appropriate for the experimenter's needs)
7. Stability over at least several months to years.

The temperature change must usually be converted into parameters that can be measured precisely with minimal noise and error, such as current, voltage, or the movement of a needle.
It should generally be used within a range where its calibration is simple; for example, the measured parameter change should be linear or fit a known easy function.

*(Image: examples of mercury, digital, dial, and gun-type thermometers)*

---

## 2. Temperature Scales and Conversions

**Conversion Table:**

| K       | °C    | °F    | °R      |
|---------|-------|-------|---------|
| 2273.16 | 2000  | 3632  | 4091.69 |
| 1773.16 | 1500  | 2732  | 3191.69 |
| 1273.16 | 1000  | 1832  | 2291.69 |
| 773.16  | 500   | 932   | 1391.69 |
| 673.16  | 400   | 752   | 1211.69 |
| 573.16  | 300   | 572   | 1031.69 |
| 473.16  | 200   | 392   | 851.69  |
| 373.16  | 100   | 212   | 671.69  |
| 273.16  | 0     | 32.0  | 491.69  |
| 233.16  | -40   | -40   | 419.69  |
| 173.16  | -100  | -148  | 311.69  |

**Conversion Formulas:**
```
°F = 32.0 + (9/5)°C
°R = (9/5)K
```
*(Figure 8.1 Relationship between Fahrenheit and Celsius temperature scales.)*

---

## 3. Mercury-in-Glass Thermometer

Uses the expansion of mercury with increasing temperature. Temperature range from 0 to about 300 °C.

*(Figure 8.4 Schematic of a mercury-in-glass thermometer. Components: Safety bulb, Capillary tube, Stem, Temperature-sensing bulb.)*

---

## 4. Gas Thermometers

### Constant-Volume Gas Thermometer
A chamber with constant volume in contact with the environment causes a change in pressure, deflecting a calibrated needle.

**Ideal Gas Law:** `pV = mRT`
**For constant volume:** `T = T_ref * (p / p_ref)`

*(Figure 8.2 Schematic of ideal-gas thermometer: a gas bulb of volume `V` at unknown temperature `T`, connected via a tube to a pressure gauge.)*
*(Figure 8.3 Results of measurements with ideal-gas thermometer: graph showing `p_ref` vs. temperature `T` is linear.)*

### Fluid-Expansion Thermometer
A vessel containing liquid and vapor connected via a capillary tube to a Bourdon pressure gauge. Temperature change causes vapor pressure change. Inexpensive, can be used over distances up to 60 meters between sensor and indicator, with 1° accuracy. Commonly used in furnace temperature measurement.

*(Figure 8.6 Fluid-expansion thermometer: vessel with vapor and liquid, connected to Bourdon gauge.)*

---

## 5. Bimetallic Strip Thermostat

Based on differential thermal expansion of two bonded materials, causing bending. Used for mechanical or digital temperature control (e.g., car engine thermostat, boilers, fan coils).

*(Figure 8.5 The bimetallic strip)*
*(Images: digital wall thermostat, car thermostat wax valve schematic, wax thermostat parts: column, piston, spring, body, temperature-sensitive wax, diaphragm)*

**Table 8.1: Mechanical properties of some commonly used thermal materials**

| Material               | Thermal Coefficient of Expansion Per °C | Modulus of Elasticity (psi) | Modulus of Elasticity (GN/m²) |
|------------------------|----------------------------------------|-----------------------------|-------------------------------|
| Invar                  | 1.7 × 10⁻⁶                             | 21.4 × 10⁶                  | 147                           |
| Yellow brass           | 2.02 × 10⁻⁵                            | 14.0 × 10⁶                  | 96.5                          |
| Monel 400              | 1.35 × 10⁻⁵                            | 26.0 × 10⁶                  | 179                           |
| Inconel 702            | 1.25 × 10⁻⁵                            | 31.5 × 10⁶                  | 217                           |
| Stainless-steel type 316| 1.6 × 10⁻⁵                             | 28 × 10⁶                    | 193                           |

**Formula for Radius of Curvature [Equation 8.5]:**
```
r = (t[3(1+m)² + (1+mn){m² + (1/mn)}]) / (6(α₂ - α₁)(T - T₀)(1+m)²)
```
Where:
- `t` : combined thickness of the bonded strip
- `m` : ratio of thicknesses of low- to high-expansion materials
- `n` : ratio of moduli of elasticity of low- to high-expansion materials
- `α₁` : lower coefficient of expansion
- `α₂` : higher coefficient of expansion
- `T` : temperature (°C)
- `T₀` : initial bonding temperature (°C)

**Example Calculation (Slide 8):**
A thermostat strip of copper and invar, each 0.3 mm thick, length 6 cm. Temperature changes from 30°C to 100°C. Find radius and deflection.

Data from Table 8.1: α₁ (Invar) = 1.7×10⁻⁶ °C⁻¹, α₂ (brass) = 2.02×10⁻⁵ °C⁻¹, E ratios: n = 147/96.5 = 1.52. m = 1.0, t = 2*(0.3×10⁻³) = 0.6×10⁻³ m, ΔT = 70°C.
```
r = (0.6×10⁻³[(3)(2)² + (1+1.52)(1+1/1.52)]) / (6(2.02-0.17)(10⁻⁵)(70)(2)²)
r = 0.132 m
```
Deflection geometry: `L = rθ` → `θ = 0.06 / 0.132 = 0.454 rad = 26.04°`
Vertical deflection `y = 2r * sin(θ/2) = 2*(0.132)*sin(13.02) = 0.0595 m`
Net deflection `d = y * sin(θ) = 0.0595 * sin(26.04) = 0.0261 m`

---

## 6. Electrical Resistance Thermometers

### 6.1 Metal Resistance Thermometers
Resistance change with temperature due to reduced electron scattering at lower temperatures. Available as wire-wound on insulating cylinder or thin-film on ceramic.

**Formula:**
`R = R₀ * (1 + aT + bT²)`
where `a`, `b` are empirical constants.
Temperature coefficient of resistance:
`α = (R₂ - R₁) / (R₁ * (T₂ - T₁))`

**Table 8.2: Resistance-temperature coefficients and resistivity at 20°C**

| Substance          | α (°C⁻¹)        | ρ (μΩ·cm) |
|--------------------|-----------------|-----------|
| Nickel             | 0.0067          | 6.85      |
| Iron (alloy)       | 0.002 to 0.006  | 10        |
| Tungsten           | 0.0048          | 5.65      |
| Aluminum           | 0.0045          | 2.65      |
| Copper             | 0.0043          | 1.67      |
| Lead               | 0.0042          | 20.6      |
| Silver             | 0.0041          | 1.59      |
| Gold               | 0.004           | 2.35      |
| Platinum           | 0.00392         | 10.5      |
| Mercury            | 0.00099         | 98.4      |
| Manganin           | 0.00002         | 44        |
| Carbon             | -0.0007         | 1400      |
| Electrolytes       | -0.02 to -0.09  | Variable  |
| Semiconductor (thermistors) | -0.068 to +0.14 | 10⁹      |

*(Graph: R/R₀ vs. temperature for Ni, Cu, Pt showing non-linear increase with temperature. Images: wire-wound platinum resistance thermometer, thin-film Pt sensor on ceramic.)*

### 6.2 Metal Resistance at Low Temperatures and Impurity Effects
Residual resistivity at 0 K due to imperfections. Total resistivity: `ρ = ρ_t + ρ_i` (thermal + impurity).  
Copper resistivity vs. temperature graph: decreases with T, approaches constant at 4.2 K (residual).  
**Five criteria for a good low-temperature resistance thermometer material:**
1. `ρ_t` should be relatively linear at higher temperatures.
2. `∂ρ/∂T` must be sufficiently large (sensitivity).
3. Linear region should extend to low temperatures (requires high purity to minimize `ρ_i`; if `ρ_i` dominates, `∂ρ/∂T → 0`).
4. Material must be formable, usually as wire.
5. If used at high temperatures or reactive atmospheres, must resist degradation.

**Low-temperature interpolation function:**
```
Z(T) = (R(T) - R(4.2 K)) / (R(273 K) - R(4.2 K))
Z(T) = A₁ + A₂*T + A₃*T² + A₄*T³ + ...
```

### 6.3 Intrinsic Semiconductors
Resistance increases as temperature drops below room temperature because carrier concentration depends on temperature. Very high resistance at low temperatures (below 10 K), with rapid changes.

**Formula:**
`ρ(T) = A * T^(-3/2) * exp(Eg / (2*kB*T))`

**Table 6.7: Resistance of a piece of intrinsic germanium**

| T (K) | R (Ω)       |
|-------|-------------|
| 295   | 920         |
| 250   | 1.40 × 10⁴  |
| 200   | 1.13 × 10⁶  |
| 150   | 1.5 × 10⁹   |
| 100   | 2.1 × 10¹⁵  |
| 80    | 7.4 × 10¹⁶  |

*(Graph: Resistivity vs. temperature, steep decrease with T. Band diagrams, holes/electrons, p-type and n-type samples.)*

### 6.4 Doped Semiconductors
Resistance vs. temperature shows a minimum around 100 K, then increases at lower temperatures.

**Carrier concentration formulas:**
- High temperatures: `n = nₑ + nₕ = 4U T^(3/2) * exp(-Eg / 2k_B T)`
- Low temperatures (doping): `n = nₑ = 2U T^(3/2) * exp(-(Eg - 2Ed) / 2k_B T)`

**Resistivity:**
`ρ(T) = 1 / σ(T) = [ e * (nₑ(T)*μₑ + nₕ(T)*μₕ) ]^(-1)`

*(Left: schematic of Fermi level shift with temperature in n-type. Right graph: log10 n vs. 1000/T showing impurity, transition, and intrinsic regions.)*

**Advantages:**
1. Doping allows use at low temperatures.
2. Large `∂ρ/∂T` gives excellent sensitivity.

**Disadvantages:**
1. `ρ(T)` function is not highly controllable; matching to calibration values is difficult.
2. Large change in `ρ` with T means one thermometer may not cover a wide temperature range; multiple sensors with different doping levels are needed (each independently calibrated).
3. Large variation with doping level makes individual calibration of each thermometer essential; two sensors with nominally the same doping can behave differently.

*(Graph: Temperature dependence of electrical resistivity for two doped silicon samples (n-type with phosphorus, p-type with boron).)*

### 6.5 Thermistors (NTC)
Semiconductor with Negative Temperature Coefficient, non-linear. Resistance decreases with increasing temperature. Usable up to 400°C.

**Formula [8.8]:**
`R = R₀ * exp[β * (1/T - 1/T₀)]`
where `R₀` is resistance at reference `T₀`, `β` is empirical constant (3500 to 4600 K).

*(Left graph: Specific resistance vs. temperature for 3 thermistor materials vs. platinum, showing sharp non-linear drop. Figure 8.8. Images: thermistor, circuit symbol, applications in radiation measurement.)*

Note: Thermistor sensitivity can detect changes of one millionth of a kelvin. Used in modern devices to measure very weak radiation intensity, replacing thermoelectric cells. Accuracy 0.01°C.

### 6.6 Carbon Resistors
Inexpensive, works over wide temperature range, good sensitivity at low temperatures.

**Formulas:**
```
log₁₀(R) + K / log₁₀(R) = A + B/T
ln(R) = A*T^(-m) + B
```

**Advantages:**
1. Very cheap.
2. Works over wide temperature range.
3. Good sensitivity at low temperatures.

**Disadvantages:**
1. Each must be individually calibrated.
2. Calibration from the formulas may not provide sufficient accuracy over a wide range.
3. Repeatability not as good as platinum or diode thermometers.
4. Resistance tends to drift even at constant temperature.

*(Graph: Resistance vs. temperature for 2.7Ω and 10Ω carbon resistors at 0.3–4.8 K. Figure 6.10. Image: 47 kΩ, 0.5 W carbon film resistor.)*

### 6.7 Diode Thermometers
Inexpensive, linear above ~30 K up to 400 K.

*(Left schematic: I-V characteristics of p-n junction, temperature dependence. Lower left: Figure 6.9 – Temperature dependence of forward bias voltage at constant current for Si and GaAs diode thermometers; linear above ~30 K. Right: Fig 1 – Simulation results for V_D and I_D at different temperatures (25, 50, 75, 100°C) and circuit diagram.)*

**Commercial types:** Example: CY670 Cryogenic Silicon Diode Temperature Sensor, range 1.4 to 500 K, price from C$908.33. Various packages and connectors shown.

---

## 7. Precision Resistance Measurement Methods

### 7.1 Four-Probe Method
Eliminates lead resistance errors. Outer probes supply current, inner probes measure voltage. Because no current flows through voltage leads, their resistance does not affect measurement.

*(Figure 1: Four probes on a sample. Figure 2: Thin sample measurement. Circuit: Current source I through Rw1, Rw4 and sample Rs2; voltmeter across Rw2, Rw3 – zero current in these leads.)*

**Resistivity formula:** `ρ₀ = (V / I) * 2πS` (S = probe spacing). For needle-like probes, an additional factor applies.

### 7.2 Wheatstone Bridge
Suitable for 1 Ω to 10 MΩ. Balance condition: galvanometer current zero, `V_AD = V_AB`.

Equations at balance:
```
I₁R₁ = I₂R₂
I₃R₃ = I₄R₄
Since I₁ = I₃ and I₂ = I₄:
R₁/R₃ = R₂/R₄   →   Rₓ = R₃ * (R₂/R₁)
```

**Measurement Errors:**
```
Limiting error: Rₓ = (R₃ ± ΔR₃) * ((R₂ ± ΔR₂) / (R₁ ± ΔR₁))
First-order: Rₓ = R₃*(R₂/R₁) * [1 ± (ΔR₁/R₁ ± ΔR₂/R₂ ± ΔR₃/R₃)]
```
**Error sources:**
1. Limiting error of known resistors
2. Insufficient detector sensitivity
3. Resistance changes due to heating (I²R) or temperature
4. Thermal emf or contact potential in the circuit
5. Lead connection error (important for low resistances)

### 7.3 Lead Resistance Compensation Methods
Circuits to reduce lead resistance effects using null methods.

*(Figure 8.7:)*
- (a) Siemens's three-lead arrangement: equal lead resistances cancel.
- (b) Callender four-lead arrangement: two lead resistances added to both unknown and reference.
- (c) Floating-potential arrangement: lead resistance in both branches.

Also, swapping right and left connections can eliminate thermal emfs in connections.

---

## 8. Thermocouples

### 8.1 Seebeck Effect
When a material experiences a temperature gradient, electron distribution changes, creating a current from hot to cold and a potential difference proportional to ΔT. The Seebeck effect is the electrical potential difference resulting from a temperature gradient. For two different materials, a thermocouple measures the potential difference between hot and cold junctions.

`ΔV = S(T) * ΔT`
`S(T)` is the thermoelectric power or Seebeck coefficient (units μV/K).

*(Image: In n-type semiconductor, temperature gradient creates electron diffusion and electric field; S = -V_th / ΔT.)*

### 8.2 Thermocouple Principle (Two Dissimilar Metals)
Junction of two metals with different Seebeck coefficients. If one junction is at a different temperature than the measurement point, a net voltage appears across A and B.

*(Figure 8.12: Junction of material 1 and material 2, with external circuit at points A, B.)*

For two rods with ΔT:
```
ΔV₁ = S₁(T) * ΔT
ΔV₂ = S₂(T) * ΔT
ΔVT = ΔV₂ - ΔV₁ = [S₂(T) - S₁(T)] * ΔT
```

### 8.3 Thermocouple Circuit and Reference Junction
Measurement uses a cold junction (reference). Voltmeter between A and B measures net voltage.

*(Figure: Circuit showing ΔV₁, ΔV, ΔV₂ contributions.)*
```
ΔVT = ΔV₁ + ΔV + ΔV₂
    = S₁(T)[ΔT + δT] - S₂(T)[δT] - S₁(T)ΔT
    = [S₁(T) - S₂(T)] δT
```
Thus output depends on δT (difference between hot and reference temperatures) and the difference in Seebeck coefficients.

*(Practical images: digital multimeter, probes, industrial thermocouple sensor with Kevlar cable.)*

### 8.4 Reference Junction at 0°C (Fixed Points)
Conventional method: place reference junctions in ice-water mixture (0°C).

*(Figure 8.15: Two methods connecting iron-constantan thermocouple to copper instrument leads with ice bath.)*

**Table 6.1: Some fixed temperature points**

| Fixed point             | Value      |
|------------------------|------------|
| Ice point              | 0°C        |
| Steam point            | 100.000°C  |
| Boiling point of sulfur| 444.600°C  |
| Freezing point of silver| 960.8°C   |
| Freezing point of gold | 1063.0°C   |
| Boiling point of oxygen| 90.18 K    |
| Triple point of oxygen | 54.36 K    |
| Boiling point of hydrogen| 20.39 K   |
| Triple point of hydrogen| 13.95 K    |
| Boiling point of helium| 4.214 K    |
| λ Point of helium      | 2.173 K    |

### 8.5 Characteristics of a Good Thermocouple
1. Stability at service temperatures (no melting or oxidation)
2. Large difference in thermoelectric coefficients: `[S₁(T) - S₂(T)]` and high `∂V/∂T = [S₁(T) - S₂(T)]`

*(Right graph: Material EMF vs. temperature for various metals relative to pure platinum. Positive: Chromel, Iron, Copper, Pt-Rh; negative: Alumel, Constantan. This guides selection of thermocouple pairs.)*

### 8.6 Commercial Thermocouple Properties

**Table 6.2: Thermocouple properties**

| Type | Connector color | Material                | Useful temp. range |
|------|-----------------|-------------------------|--------------------|
| T    | Blue            | Copper / constantan     | -200 to 350°C      |
| E    | Violet          | Chromel / constantan    | -200 to 900°C      |
| J    | Black           | Iron / constantan       | 0 to 750°C         |
| K    | Yellow          | Chromel / alumel        | -200 to 1250°C     |
| G    | Red/green       | W / W+26%Re             | 0 to 2300°C        |
| C    | Red             | W+5%Re / W+26%Re        | 0 to 2300°C        |
| D    | Red/white       | W+3%Re / W+25%Re        | 0 to 2300°C        |
| R    | Green           | Pt / Pt+13%Rh           | 0 to 1450°C        |
| S    | Green           | Pt / Pt+10%Rh           | 0 to 1450°C        |
| B    | White           | Pt+6%Rh / Pt+30%Rh      | 0 to 1700°C        |

*(Positive wire underlined. Right graph: Figure 6.4 – Thermoelectric powers for some thermocouple pairs at low temperatures, 1–300 K.)*

---

## 9. Optical and Radiation Thermometry

### 9.1 Blackbody Radiation Theory
Temperature dependence of emission spectrum.

**Planck's law (energy density):**
`E(ω) dω = (ħ * ω³ * dω) / (4π² * c² * (e^(ħω / kB*T) - 1))`

**Stefan-Boltzmann law (total radiated energy):**
`∫ E(ω) dω = σ * T⁴`

*(Left graph: Planck distribution for bodies at 1200 K and 1800 K; peak shifts to higher frequencies with T, visible region marked. Right graph: Spectra of black body, gray body, and nongray body at same temperature.)*

### 9.2 Optical Pyrometer
*(Figure 6.13 Schematic diagram of optical pyrometer: object, lens, aperture, high-temperature filter, tungsten lamp, red filter, lens, aperture, eyepiece, observer, current source.)*

**Principle:** Match brightness of hot object with that of a calibrated tungsten filament by adjusting current. The filament "disappears" when brightness matches.

*(Image with three states: 1. filament dark (cooler than source), 2. filament bright (hotter), 3. filament vanishes (matched). Right: pyrometer schematic with object, lens, filter, filament, power supply, scale, eyepiece.)*

### 9.3 Emissivity Error – Example 8.8
**Problem:** Radiation from a metal piece measured, temperature determined as 1050°C assuming emissivity 0.82. Actual emissivity is 0.75. Calculate error.

Radiated energy: `q/A = εσT⁴`
Using T = 1323 K, ε = 0.82, find real T' with ε'=0.75:
```
(0.82) * (1323)⁴ = (0.75) * (T')⁴
T' = 1323 * (0.82 / 0.75)^(1/4) = 1352 K
Error ΔT = 1352 - 1323 = 29°C
```
Comment: A relatively large error in emissivity (0.82 vs 0.75) causes a smaller error in temperature (2.1% difference). Near room temperature (300 K), error would be about 6°C.

### 9.4 Digital Radiation Thermometer
*(Links to videos. Image: gun-type thermometer displaying 103.4°F, with colored body temperature indicators.)*

### 9.5 Emissivity Table and Correction
**Table 6.8: Emissivities of some materials at 6550 nm (solid and liquid states)**

| Material | ε(solid) | ε(liquid) |
|----------|----------|-----------|
| Cr       | 0.34     | 0.39      |
| Co       | 0.36     | 0.37      |
| Cu       | 0.10     | 0.15      |
| Au       | 0.14     | 0.22      |
| Fe       | 0.35     | 0.37      |
| Mn       | 0.59     | 0.59      |
| Mo       | 0.37     | 0.40      |
| Ni       | 0.36     | 0.37      |
| Pd       | 0.33     | 0.37      |
| Pt       | 0.30     | 0.38      |
| Rh       | 0.24     | 0.30      |
| Ag       | 0.07     | 0.07      |
| Ti       | 0.63     | 0.65      |
| W        | 0.43     | —         |

*(Figure 6.16: Temperature correction (°C) vs. measured temperature (°C) for various emissivities (0.2 to 0.9) at 655 nm; correction increases with lower emissivity and higher temperature.)*

---

## 10. Calibration of Thermometers

Periodic calibration is necessary. A trusted reference thermometer covering the range is brought into thermal equilibrium with the sensor under test at multiple temperature points. More data points are better unless a known function applies (e.g., linear requiring two points). For linear functions, fixed points are used: triple point of water (0.01°C), ice-water mixture (0°C at atmospheric pressure), boiling pure water (100°C), liquid nitrogen, and other fixed points.

**ITS-90 Fixed Points:**
- Boiling point of Nitrogen: -195.798°C
- Mercury triple point: -38.8344°C
- Triple point of water: 0.01°C
- Melting point of Gallium: 29.7646°C
- Freezing point of Indium: 156.5985°C
- Freezing point of Tin: 231.928°C
- Freezing point of Lead: 327.462°C
- Freezing point of Zinc: 419.527°C
- Freezing point of Antimony: 630.63°C
- Freezing point of Aluminium: 660.323°C
- Freezing point of Silver: 961.78°C

*(Image: Multi Function Calibrator with temperature source, master sensor and sensor under test, and inbuilt indicator.)*