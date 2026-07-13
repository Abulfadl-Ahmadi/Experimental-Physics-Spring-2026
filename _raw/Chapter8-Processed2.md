# Low-Temperature Technology

## Course Information
- **Course:** Experimental Methods in Physics  
- **Instructor:** Azam Irajizad  
- **Year:** 1405 (Iranian calendar)  
- **Note:** The materials are for students of this course only, compiled from accessible references such as Wikipedia, manufacturers’ catalogs, textbooks, and personal experience. Do not distribute outside the class.

---

## Applications of Science and Technology of Refrigeration
Where and for what purpose do we apply refrigeration? Some applications of the science and technology of refrigeration:
1. Investigation of physical properties of materials that undergo phase changes at low temperatures, such as superconductivity.
2. Laboratory investigation of phenomena that require the elimination of thermal noise, e.g., the quantum Hall effect.
3. In engineering, for shaping solids.
4. For creating a very good vacuum.
5. In medicine, for preserving genes, sperm, or organ transplants, and wound treatment.
6. In the food and agricultural industries for long-term preservation of products.
7. In submarine and rocket fuels.
8. Where strong magnetic fields are needed, such as MRI or magnetic levitation (e.g., high-speed trains).

*Illustrations:* Image of a superconducting block above a holder, an MRI machine, and a high-speed magnetic levitation (maglev) train.

---

## Methods of Refrigeration and Cryogenic Fluid Properties

### Refrigeration Methods
1. Contact with cold solids or liquids – simple if cold liquids are available.
2. Use of refrigerators (refrigerants) based on cold liquids, closed cycles, and magnetic salts.
3. Use of lasers.
4. Peltier-effect coolers.

### Phase Diagram (General)
A pressure–temperature phase diagram shows solid, liquid, gas phases, triple point (TP), critical point (CP), and relevant phase boundaries.

### Table 7.1: Properties of Cryogens
| Cryogen | Triple point (K) | Normal boiling point (K) | Critical point (K) |
|---------|------------------|--------------------------|---------------------|
| Methane | 90.7             | 111.6                    | 190.5               |
| Oxygen  | 54.4             | 90.2                     | 154.6               |
| Argon   | 83.8             | 87.3                     | 150.9               |
| Nitrogen| 63.1             | 77.3                     | 126.2               |
| Neon    | 24.6             | 27.1                     | 44.4                |
| Hydrogen| 13.8             | 20.4                     | 33.2                |
| Helium  | 2.2*             | 4.2                      | 5.2                 |

* The asterisk denotes the lambda point (λ point).

---

## Joule–Thomson Effect and Gas Liquefaction

### The Joule–Thomson (Joule–Kelvin) Effect
In thermodynamics, the Joule–Thomson effect describes the temperature change of a gas or liquid when it is forced through a valve or porous plug while being perfectly insulated so that no heat is exchanged with the environment (a throttling process). This effect is named after James Prescott Joule and William Thomson.

*Illustration:* An industrial valve with high‑pressure gas inlet (900 psi) and outlet (200 psi) labeled “Joule‑Thomson Effect.” Inlet temperature 80 °F, outlet 30 °F.

**Warning:** If the valve of a compressed nitrogen cylinder at 298 K is fully opened, frost forms around the valve, indicating that the valve temperature falls below the freezing point of water. A similar experiment with hydrogen, which heats upon expansion, can lead to an explosion!

### Mathematical Proof of the Joule–Thomson Effect (Insulated Tube)
Diagram shows an insulated tube with a left piston (high pressure), a porous plug in the middle, and a right piston (low pressure). Initial gas volume \(V_1\), final volume \(V_2\).

\[
w = w_{\text{left}} + w_{\text{right}} = -\int_{V_1}^{0} P_1\,dV - \int_{0}^{V_2} P_2\,dV = P_1 V_1 - P_2 V_2 \quad (1)
\]
Since the tube is insulated, \(q = 0\), so:
\[
\Delta U = U_2 - U_1 = w = P_1 V_1 - P_2 V_2 \quad (2)
\]
Rearranging:
\[
U_2 + P_2 V_2 = U_1 + P_1 V_1 \quad \Rightarrow \quad H_2 = H_1 \quad (3)
\]
**Conclusion:** Enthalpy remains constant in a Joule–Thomson process (\(H_2 = H_1\)).

### Joule–Thomson Coefficient (Constant Enthalpy)
The process is isenthalpic. This model is used for nitrogen and hydrogen.

**Definition:**
\[
\mu_{J-T} = \lim_{\Delta P \to 0} \left( \frac{\Delta T}{\Delta P} \right)_H = \left( \frac{\partial T}{\partial P} \right)_H
\]
Simple form:
\[
\mu_{JT} = \frac{T_2 - T_1}{P_2 - P_1}
\]

From differential enthalpy:
\[
dH = C_p\,dT + \left( \frac{\partial H}{\partial P} \right)_T dP = 0 \quad (5)
\]
\[
C_p \left( \frac{\partial T}{\partial P} \right)_H + \left( \frac{\partial H}{\partial P} \right)_T = 0 \quad \Rightarrow \quad \left( \frac{\partial H}{\partial P} \right)_T = - C_p \mu_{J-T} \quad (6)
\]

### Dependence of the Joule–Thomson Coefficient on Volume, Heat Capacity, Thermal Expansion Coefficient, and Temperature
Fundamental thermodynamic relation for enthalpy:
\[
dH = T\,dS + V\,dP
\]
Differentiate with respect to \(P\) at constant \(T\):
\[
\left( \frac{\partial H}{\partial P} \right)_T = T \left( \frac{\partial S}{\partial P} \right)_T + V
\]
Using the Maxwell relation:
\[
\left( \frac{\partial S}{\partial P} \right)_T = - \left( \frac{\partial V}{\partial T} \right)_P = - V \alpha
\]
where \(\alpha\) is the cubic coefficient of thermal expansion.

Substituting:
\[
\mu_T = -T V \alpha + V
\]
Final expression:
\[
\mu_{JT} \equiv \left( \frac{\partial T}{\partial P} \right)_H = \frac{V}{C_p} (\alpha T - 1)
\]
This formula expresses the Joule–Thomson coefficient in terms of measurable properties: heat capacity \(C_p\), molar volume \(V\), and thermal expansion coefficient \(\alpha\). The inversion temperature (\(\mu_{JT}=0\)) occurs when \(\alpha T = 1\).

### Inversion Temperature Graph and Table
**Question:** Which gases can be cooled from room temperature using this method?

The coefficient depends on the gas type and its temperature and pressure before expansion.

**Graph:** Joule–Thomson coefficient (K/bar) vs. temperature (K) for H₂, N₂, Ar, CO₂, He. CO₂ has a positive coefficient; H₂ and He have negative coefficients at high temperatures. The inversion point where the sign changes is indicated.

**Cooling condition table:**
- If gas temperature < inversion temperature → \(\mu_{JT} > 0\). Since \(\delta P\) is always negative (pressure decreases), \(\delta T\) is negative → **gas cools**.
- If gas temperature > inversion temperature → \(\mu_{JT} < 0\). Since \(\delta P\) is negative, \(\delta T\) is positive → **gas heats**.

### Inversion Temperature of Real Gases
**Definition:** The temperature at which the sign of the Joule–Thomson coefficient changes. All real gases have an inversion point; its value depends on the pressure before expansion.

The inversion temperature lies on the boundary of the temperature–pressure curve. At a given pressure, a constant‑pressure line cuts the inversion curve at two points: the lower and upper inversion temperatures. Outside this interval \(\mu < 0\); inside the interval \(\mu > 0\).

**Graphs:**
- Left: Inversion curve on a \(T\)–\(P\) diagram with shaded region \(\mu > 0\) and unshaded \(\mu < 0\).
- Right: Inversion curves for N₂ (blue), H₂ (red), and He (purple). For N₂ upper inversion ~621 K, lower ~120 K; H₂ upper ~204 K, lower ~33 K; He upper ~40 K.

**Summary:**
- \(\mu > 0, \ P\downarrow, \ \Delta P < 0, \ \Delta T < 0\) → temperature decreases.
- \(\mu = 0, \ P\downarrow, \ \Delta P < 0, \ \Delta T = 0\) → no change.
- \(\mu < 0, \ P\downarrow, \ \Delta P < 0, \ \Delta T > 0\) → temperature increases.

### Gas Liquefaction Differences
Left graph: \(T\)–\(P\) diagram showing gas, supercritical, and liquid regions with \(\mu_{JT} > 0\) and \(\mu_{JT} < 0\) domains.  
Right graph: Inversion curves for N₂, H₂, He on \(T/K\) vs. \(p/\text{atm}\). The green area inside the curve corresponds to \(\mu_{JT} > 0\) (cooling). Vertical lines indicate upper and lower inversion temperatures.

---

## Refrigeration Cycles and Industrial Refrigerators

### Working Principle of Household and Industrial Refrigerators (Based on the Joule–Thomson Effect)
**Seven‑step cycle:**
1. The refrigerant gas is compressed to increase pressure, usually by a positive‑displacement compressor.
2. The compressed gas is sent to the condenser to remove superheat and turn it into liquid.
3. The compressed, liquefied refrigerant passes through an expansion valve (JT valve).
4. Rapid expansion across the JT valve cools the gas.
5. The cold gas is sent to a heat exchanger where it cools other fluids (water, air, etc.).
6. In this process, the refrigerant itself warms up.
7. It is then collected and returned to the compressor (step 1). The refrigeration cycle continues.

**Diagrams:**  
- Vapor‑compression refrigeration cycle: compressor → condenser → JT valve → evaporator.  
- Simplified cycle divided into high‑pressure and low‑pressure sides.

### Industrial Refrigerators and Refrigerants
Various schematic diagrams: simple refrigeration cycle, two‑stage cycle, automotive air‑conditioning system, and industrial refrigeration system.

**Automotive AC system (right diagram):**
1. Compressor
2. Compressor Clutch
3. Condenser
4. Condenser Fan
5. Receiver/Drier
6. Expansion Valve
7. Evaporator
8. Dash Blower Motor

Color‑coded lines: red (high‑pressure hot gas), yellow (high‑pressure liquid), dark blue (low‑pressure liquid/vapor mix), light blue (low‑pressure cold vapor).

---

## Liquid Nitrogen: Properties, Production, and Air Separation

### Properties of Liquid Nitrogen (and Liquid Air)
Liquid nitrogen at atmospheric pressure boils at 77 K. It is colorless, odorless, and transparent like water. It can be stored in insulated containers. In contact with air it freezes nitrogen or air. It is used in medicine for cryotherapy (e.g., wart and cataract treatment, painless, outpatient). If liquid air is used, note that upon warming, nitrogen evaporates first, leaving oxygen enriched liquid, which can be hazardous. (Liquid nitrogen can be further cooled and solidified by pumping.)

**Air composition (pie chart):**
- Nitrogen: 78.08%
- Oxygen: 20.95%
- Argon: 0.93%
- Others: Neon 0.0018%, Helium 0.0005%, Krypton 0.0001%, Hydrogen 0.00005%, Xenon 0.000009%, Carbon dioxide 0.038%.

### Production Methods for Liquid Nitrogen
One of the oldest methods is fractional distillation of air, invented by German engineer Carl von Linde. High‑purity air in large tonnage is compressed; simultaneously, impurities such as water vapor and CO₂ are removed. The air is cooled through heat exchangers and passed through expansion valves and turbines to reach cryogenic temperatures, then liquefied. The liquid air is sent to a distillation column with several trays to separate nitrogen, oxygen, and argon. Each element is drawn off at its distillation point to ensure maximum purity. Liquid nitrogen produced this way has **99.999%** purity.

**Diagram:** Full process chart of an air separation plant showing filters, air compressor, reversing heat exchangers, coolers, upper and lower distillation columns, expansion turbine, and storage tanks for gas/liquid oxygen, nitrogen, and argon.

### Separation of Nitrogen and Oxygen from Liquid Air
1. Air enters a **compressor** operating at **–200 °C**.
2. Passes through a **filter** to remove trace gases and water.
3. Enters the **fractionating column**:
   - From the top: **nitrogen** gas at **–196 °C**.
   - From the bottom: liquid **oxygen** at **–183 °C**.

---

## Liquid Hydrogen: Production and Applications

### Liquid Hydrogen
**Hazard labels:** Flammable gas, flammable liquid, UN number 1966 (Liquid Hydrogen).

For liquefaction, purified hydrogen gas is compressed, cooled, and expanded in several stages, each time getting colder. When the gas expands near its boiling point of **–253 °C**, part of it condenses as liquid hydrogen and is collected in a separate container; the remaining gas is returned to the cycle.

**Diagram:** Simplified schematic of a hydrogen liquefier based on the Joule–Thomson effect: Hydrogen gas → compression → pre‑cooling (with liquid nitrogen) → cryogenic cooling (with helium) → expansion and separation → liquid hydrogen.

Images: large white liquid hydrogen storage tank labeled “HYDROGEN”, and a submarine (illustrating use in submarine fuel).

### Liquid Hydrogen as Rocket Fuel (NASA SLS System)
Liquid hydrogen is a common rocket fuel. Both NASA and the U.S. Air Force have numerous LH₂ tanks with a capacity of 3.8 million liters (1 million gallons). In most rocket engines using LH₂, the nozzle and other components are first cooled before mixing with the oxidizer (usually liquid oxygen, LOX), and then combustion produces thrust.

**Infographic: Inside the SLS Core Stage**
- Height: 212 ft, diameter: 27.6 ft, weight with fuel: 2.3 million pounds.
- **Engine section:** delivers fuel to 4 RS‑25 engines.
- **Liquid hydrogen (LH₂) tank:** holds 537,000 gallons of LH₂ cooled to **–423 °F**.
- **Intertank:** houses electronics, computers, booster attachment points.
- **Liquid oxygen (LOX) tank:** holds 196,000 gallons of LOX cooled to **–297 °F**.
- **Forward skirt:** contains computers, navigation system, the “brain” of the rocket.
- Four engines produce 2 million pounds of thrust. The tanks together hold 733,000 gallons of LH₂ and LOX, enough to fill 63 large tanker trucks.

---

## Helium Liquefaction: Hampson–Linde Cycle

### Hampson–Linde Cycle for Liquid Helium
Cooling helium gas with liquid nitrogen down to 77 K is possible, but to reach ~4 K the temperature must be drastically lowered. Can the Joule–Thomson effect do it?

**Cycle description:**
- Compressed gas is sent to a cooling environment (liquid nitrogen).
- The cooled gas exits the final cooling stage and passes through a counter‑flow heat exchanger.
- It then expands through a throttle valve and cools further.
- At this point the gas is at low pressure and at its coldest in the current cycle. The portion that liquefies becomes the liquid helium product.
- The remaining low‑pressure gas is directed through the counter‑flow heat exchanger to cool the incoming high‑pressure gas, then returns to the compressor.

Diagrams: Simple cycle with compressor, condenser, heat exchanger, expansion valve, evaporator; schematic of a helium liquefier with 200 bar input, main heat exchanger, expansion valve, liquid air bath, and 20 bar output.

---

## Properties of Liquid Helium and Superfluidity

### Properties of Liquid Helium
At standard pressure, helium exists as a liquid only at very low temperatures: **–269 °C** (4.15 K). The boiling point and critical point depend on the isotope: common helium‑4 or rare helium‑3. Density of liquid helium‑4 at its boiling point and 1 atm (~101.3 kPa) is about 125 g/L (about 1/8 the density of liquid water).

**Table 7.3: Liquid helium required to cool 1 kg of copper from 77 K to 4.2 K**
- Method 1 (using latent heat of vaporization): **2.3 liters** of helium.
- Method 2 (using gas heat capacity + latent heat): **0.14 liters** of helium.

**Phase diagram of helium:** Pressure vs. temperature. Shows solid, liquid, gas, and a **superfluid** region (near 2.2 K). The liquid–gas curve indicates the critical point at ~5.2 K and the lambda line (liquid–superfluid boundary).

### Superfluidity
A superfluid is a state of matter in which the fluid behaves with **zero viscosity and zero entropy**. Typically hydrogen, helium‑3, and helium‑4 at the “lambda point” exhibit zero viscosity. Superfluids, like superconductors, show no resistance to flow; they move without any friction (making it very hard to create pressure or temperature differences). Similarly, it is difficult to create a potential difference.

**Special superfluid effects:**
- **Fountain effect:** If a capillary tube is placed in a superfluid helium bath and heated (even by shining light on it), helium climbs up the tube (according to the Clausius–Clapeyron equation).
- **Superfluid film effect:** Superfluid helium can form an atomic film and climb over the walls of its container.

**Diagrams:**
- Specific heat capacity (\(C_s\) [J/gK]) vs. temperature (K) showing a sharp peak at ~2.2 K (the lambda point, \(T_\lambda\)).
- U‑shaped container illustration showing superfluid helium creeping up the walls and over the edge.

---

## Cryostat Design and Operation

### Liquid Nitrogen Cryostat (Design)
**Figure 7.2: Simple LN₂ cryostat** with electrical feedthrough, vacuum system connection, cover, liquid nitrogen, probe, Dewar, and experiment section. Regions 1, 2, 3 are marked.

**Design notes:**
- The container holding LN₂ at 77 K must be thermally isolated from the outer body. A good insulator is a vacuum with superinsulation.
- The object under test must be in thermal contact with the LN₂. Therefore, the sample chamber is first evacuated and then back‑filled with helium or nitrogen exchange gas.
- Due to slow boil‑off of LN₂ (from weak heat inleak), the gas pressure above the liquid rises. A pressure relief valve must be provided to prevent rupture.

### Operation and Measurement Steps
1. Initially, regions 1, 2, 3 are at room temperature and laboratory pressure.
2. The sample is placed in position and electrical connections are made.
3. Regions 1 and 3 are evacuated (vacuum).
4. Liquid nitrogen is introduced into region 2.
5. Nitrogen or helium exchange gas is admitted into region 1.

**Questions:**
- What happens if we do not evacuate region 1 first, and why?
- If we want to return the sample temperature from 77 K to room temperature, what should we do?

### Cold‑Finger Cryostat
**Figure 7.3:** Two types of LN₂ cryostats using a “cold finger” arrangement.  
(a) A copper cold finger immersed in LN₂ connects to the experiment section above.  
(b) The experiment section is below, and the cold finger extends downward from the LN₂ reservoir.

The sample is attached to the cold end of a metal with high thermal conductivity (e.g., copper) that is immersed in (or in contact with) liquid nitrogen. To cool the sample, the chamber is first evacuated and the copper piece is placed in thermal contact with the LN₂ container.

### Liquid Helium Cryostat
**Figure 7.4:** A Dewar‑type liquid helium cryostat with an intermediate liquid nitrogen jacket. Labeled: helium fill port, vacuum connections, helium vent, baffle shields, vacuum space, liquid nitrogen, liquid helium, exchange gas space, sample region, and bottom of the reservoir. Regions 1–5 are indicated.

**Step‑by‑step operation:**
1. Region 1: insulation, 2: LN₂, 3: insulation (vacuum), 4: LHe space, 5: sample chamber.
2. Initially everything is at room temperature and atmospheric pressure.
3. All chambers are evacuated.
4. LN₂ is poured into regions 2 and 3 (cooling sample to 77 K).
5. Region 3 is evacuated to break thermal contact.
6. Liquid helium is transferred into region 4; the sample cools to 4.2 K.
7. To warm the sample, an electrical heater (simple wire coil) can be used for temperature control.
8. Lids and walls must be insulating and thermally reflective to minimize heat inleak.
9. LN₂ and LHe reservoirs must have open vent valves. To warm the sample, it must be removed from the LHe source under low‑pressure helium gas and slowly brought above 0 °C before the chamber can be opened.

### Needle‑Valve Helium Cryostat
A simple cryostat with an outer LN₂ jacket and an inner LHe chamber. A needle valve (throttle valve) and a capillary tube allow a small amount of LHe to leak into the sample chamber at lower pressure. The cold gas can lower the temperature below 4 K. (The exiting helium gas is usually collected and re‑liquefied in an external closed system.) The system is shielded by vacuum/superinsulation, LN₂ at 77 K, and the inner LHe chamber.

### Transfer of Liquid Helium or Nitrogen
Transfer by pressure difference and siphon. The transfer line must be flexible and well insulated.

**Figure 7.6:** LHe transfer arrangement: storage Dewar, transfer tube, cryostat, valve, vent.  
**Figure 7.7:** A stainless‑steel LHe transfer tube (by G.K. White) with copper refrigeration tube, nylon fishing line, stainless steel tube, and Inconel tube.

---

## Level Sensing in Cryogenic Dewars

### Diaphragm/Sound Method
**Figure 7.14:** Liquid helium level indicator: (a) thin metal cup, (b) elastic diaphragm, (c) long tube. A real instrument photo is shown alongside. Two conceptual diagrams show helium bubbles in a container as a sign of boiling.

- A funnel‑shaped metal piece with a plastic diaphragm and a long tube is inserted as deep as possible into the reservoir.
- Boiling LN₂ or LHe creates bubbles, causing noise and impacts on the elastic diaphragm, which can be felt by placing a finger on the cover.
- The tube is pulled up until the impacts cease, indicating that the tube has been raised above the liquid surface.

### Superconducting Level Sensor
**Figure 7.15:** Superconducting LHe level indicator: (a) outer shell, (b) superconducting wire, (c) resistive heater, (d) non‑superconducting lead wires, (e) insulating end caps, (f) liquid entry holes.

A long superconducting wire is inserted into the chamber. By measuring resistance, one can estimate the helium level. If the resistance is very low, it means the tank is full and the wire is immersed in the liquid superconductor.

### Cylindrical Capacitive Level Sensor
**Figure 7.16:** Capacitive LN₂ depth sensor: (a) top cover, (b) outer stainless‑steel tube, (c) inner stainless‑steel tube, (d) spacers, (e) electrical connections. A side diagram shows a cylindrical tank with a level sensor, a reference sensor in liquid, and an air sensor.

A cylindrical capacitor whose capacitance changes as liquid enters; it can be calibrated.

---

## Temperature Control Methods

1. **Method 1:** Using a heater (wire carrying electric current) and a thermometer (thermistor or thermocouple) to build a control circuit that compares and adjusts the temperature to the desired setpoint.
2. **Method 2:** Using the pressure–temperature dependence of a cold liquid’s vapor. By controlling the vapor pressure above the liquid, one can control the temperature, using vapor pressure–temperature tables (Table 7.4) for boiling points and below.

**Table 7.4: Vapor Pressure of Gases** (pressure in mmHg vs. temperature in K for ⁴He, H₂, N₂, O₂). Example: at 100 mmHg, temperatures are ⁴He 2.632 K, H₂ 15.18 K, N₂ 63.03 K, O₂ 74.07 K.

### Manostat Structure for Pressure Control
**Figure 7.18 (left):** Cartesian manostat with mercury, rubber pad, and valve G.  
**Figure 7.19 (right):** Bellows manostat with pump, vapor outlet, and flexible bellows.

- Left: Valve G is adjusted; a rubber pad is in equilibrium. If pressure rises, the rubber pad with mercury rises, opening the vent further; if pressure falls, the pad lowers and the vent closes more.
- Right: An accordion‑like bellows acts as a reservoir; opening and closing the pump path keeps pressure constant.

### Electronic Temperature Controller Suitable for All Temperatures
Heater current is adjusted by a set voltage using a comparator.

**Figure 7.20 (left):** Temperature controller using a thermistor. A Wheatstone bridge with \(R_1, R_2\), thermistor \(R_{th}\), and set resistor \(R_{set}\). The bridge output goes to an amplifier connected to a heater and a diode.  
If \(R_{th} \neq R_{set}\), the bridge voltages are unequal, and the amplifier gives an output. When heating is needed (temperature too low, \(R_{th} > R_{set}\)), the amplifier output is negative and the diode conducts current to the heater. If the sample is too hot (\(R_{th} < R_{set}\)), the amplifier output is positive and the diode blocks current. For sensors with positive temperature coefficient (e.g., platinum), the diode direction must be reversed.

**Figure 7.21 (right):** Temperature controller using a thermocouple. The thermocouple voltage is compared by a differential amplifier against a reference voltage from a voltage divider.

---

## Closed‑Cycle Helium Refrigerator (Stirling Cycle)

Closed‑cycle helium cryostats do not need refilling and can operate indefinitely. Objects may be cooled by attachment to a cold metal plate inside a vacuum chamber that is in thermal contact with the helium chamber.

### Ideal Stirling Cycle
The ideal Stirling cycle consists of four thermodynamic processes on the working fluid:
I. 1→2: Isothermal heat addition (expansion).  
II. 2→3: Isochoric heat removal (constant volume).  
III. 3→4: Isothermal heat removal (compression).  
IV. 4→1: Isochoric heat addition (constant volume).

**P–V diagram:** Shows the cycle with high temperature \(T_H\) and low temperature \(T_C\).

**Equipment components:** Compressor, cooling water connections, vacuum pump, vacuum valve, expansion unit, radiation shield, vacuum cover, sample holder, and a temperature controller.

### Stirling Cycle Details (Achieving ~5 K)
**Cross‑section of a Stirling refrigerator:** high‑pressure gas inlet, low‑pressure gas return, rotary valve motor, surge volume, valve, valve stem, displacer, first‑stage regenerator, first‑stage heat station, second‑stage regenerator, second‑stage heat station.

**Four stages:**
- **First:** The closed‑cycle cryostat begins by the rotating valve disk opening the high‑pressure path, allowing helium gas to flow through the regenerator material into the expansion space.
- **Second:** The pressure difference causes the displacer to move “up,” allowing the gas at the bottom to expand and cool.
- **Third:** The next rotation of the valve disk opens the low‑pressure path, allowing the cold gas to flow back through the regenerator, removing heat from the system.
- **Fourth:** Finally, the pressure difference returns the displacer to its original position, completing the cycle.

---

## Sub‑4.2 K Cooling: Pumped Helium‑4 and Helium‑3

### Achieving Temperatures from 4.2 K down to 1.3 K by Pumping on Liquids
A liquid helium bath (LHe bath) and a small ⁴He pot connected to a helium pump. Temperature ~1 K.  
Right: Vapor pressure curve (mbar vs. K) for ³He and ⁴He. At very low temperatures, ³He has much higher vapor pressure than ⁴He.

Liquid can be injected through a narrow tube from the helium reservoir into a small pot, then pumped away as gas and returned to the storage/liquefaction cycle. By pumping on liquid ⁴He, one can reach about 1 K (colder than interstellar space). If ³He is used, temperatures down to **0.25 K** are attainable.

---

## Dilution Refrigeration (³He/⁴He)

### Millikelvin Temperatures with Helium‑3 and Helium‑4
- Helium‑4 is a boson, helium‑3 is a fermion.
- Natural helium contains ³He at about 1 part in 100,000.
- ³He can be artificially produced from hydrogen via the nuclear reaction: \(_1^3H \rightarrow _2^3He + e^-\).
- ³He is more expensive than ⁴He and is used alone or in mixtures to reach millikelvin temperatures.

**Phase diagram of ³He/⁴He:** Temperature vs. ³He concentration.
- Green region: normal fluid ⁴He/³He mixture.
- Yellow region: Fermi liquid ³He in superfluid ⁴He.
- Red region (bottom): forbidden region.
- Pink region (further below): phase separation.

The phase curve shows that below the tricritical point the mixture separates into two phases: one rich in ³He (concentrated phase) and one dilute in ³He in ⁴He (dilute phase). To reach low temperatures, ³He must be extracted from the dilute phase.

### Principles of the ³He/⁴He Dilution Refrigerator
First, at 4 K the mixture is introduced into the container and cooled to 1 K. At this temperature the liquid mixture separates into a ³He‑rich phase (lighter) and a ⁴He‑rich phase (heavier). Increasing the concentration of the upper phase reduces its density, and the lower phase moves toward higher ⁴He concentration. For cooling, ³He is extracted from the mixing chamber and transferred to the still.

### Structure of a Dilution Refrigerator
**Detailed diagram (left):**
- LN₂ bath 77 K
- LHe bath 4.2 K
- ³He pump inlet and purification system
- Condenser
- Still with heater
- Main impedance ~600 mK
- Heat exchangers
- Secondary impedance
- Mixing chamber with phase boundary (concentrated phase and dilute phase)
- Sample under test (DUT/Sample) at ~20 mK.

**Description:** The ⁴He/³He dilution refrigerator provides continuous cooling down to ~20 mK. The idea was first proposed by Heinz London in the early 1950s and experimentally realized in 1964 at the Kamerlingh Onnes Laboratory, Leiden University. ³He evaporated from the mixed phase is pumped away at about 1 K and condensed on contact with the still. Liquid ³He passes through heat exchangers, makes thermal contact with the colder mixture in the mixing chamber, and after passing through the phase boundary, the resulting dilution of ³He into the dilute phase absorbs heat, cooling the mixing chamber. Achievable temperature: ~20 mK.

### Physical Assembly of a Dilution Refrigerator
Left: A copper/stainless‑steel cylindrical dilution unit for operations below 10 mK, with silver connections, sintered silver heat exchangers, and mixing chamber at bottom.  
Middle: Internal assembly of a cryogen‑free dilution refrigerator, with temperature stages labeled (60 K, 4 K, 0.7 K, 100 mK, 10 mK). Overall height 710 mm, width 240 mm.  
Right: Simplified diagrams showing still, heater, pump, mixing chamber, and heat exchangers; phases and phase boundary indicated.

---

## Magnetic Cooling (Adiabatic Demagnetization)

### Magnetic Refrigeration
**Left diagrams:**
- Top left: Adiabatic magnetization and adiabatic demagnetization (cycles of raising/lowering magnetic field \(H_0\)).
- Bottom left: Reverse Carnot cycle in entropy–temperature space for magnetic processes. Magnetic field varies from 0 to 8 T. Steps: 1→2 adiabatic magnetization, 2→3 isothermal magnetization, 3→4 adiabatic demagnetization, 4→1 isothermal demagnetization.

**Principles:**
- **Adiabatic magnetization:** In a thermally insulated environment, applying a magnetic field aligns the magnetic dipoles, reducing magnetic entropy and heat capacity.
- **Isomagnetic enthalpy transfer:** The added heat can then be removed by a fluid or gas (e.g., liquid helium). Then the magnetic field is removed adiabatically.
- **Adiabatic demagnetization:** The material is removed from the magnetic field under adiabatic conditions, keeping total entropy constant. The magnetic field decreases, thermal energy decreases, magnetic orientations become disordered again, and the sample cools. This process can continue down to millikelvin temperatures.

---

## Thermoelectric Cooling (Peltier Effect)

### Peltier‑Effect Cooling
Thermoelectric coolers (Peltier modules) have two sides; when a DC electric current passes through the device, it transfers heat from one side to the other, making one side colder and the other hotter. The “hot” side is attached to a heat sink to stay at ambient temperature, while the cold side can reach room temperature or below. In special applications, multiple coolers can be stacked for lower temperatures, though overall efficiency drops significantly.

**Advantages:** No moving parts, very long lifetime, small size, easy to shape.  
**Disadvantages:** High cost and poor efficiency for a given cooling capacity.  
**Applications:** Computer component cooling, water coolers.

**Model naming guide:** Example **TEC1‑12709**
- TEC: ThermoElectric Cooler
- 1: number of stages (typical=1)
- 12: size (rated current 6–9 A)
- 7: number of P‑N pairs (highly doped semiconductors)
- 09: current rating

---

## Laser Cooling and Magneto‑Optical Trap

### Laser Cooling
**Diagrams:**
- (a) An atom moving toward a laser source absorbs a laser photon. (b) Absorption equalizes the photon and atom momentum, reducing the atom’s speed. (c) The atom spontaneously emits a photon in a random direction, further reducing the average velocity.
- Doppler effect formula for light: \(V_{\text{observed}} = V_{\text{source}} \sqrt{\frac{1 + \frac{v}{c}}{1 - \frac{v}{c}}}\)

If laser light shining on an atom has energy equal to or greater than the energy difference between two atomic levels, it is absorbed (otherwise not). An atom moving toward or away from the source experiences a Doppler shift, increasing or decreasing the frequency. By tuning the laser frequency so that only atoms moving toward the laser absorb energy, and because they re‑emit in all directions, the momentum and thus the speed and temperature decrease. By shining lasers from all directions on a collection of atoms or ions, one can reduce their speed and temperature.

### Magneto‑Optical Trap (MOT)
**Diagrams:**
- Left: Six red laser beams converging from ±x, ±y, ±z directions onto a central cloud of atoms; atoms are compressed by a central force.
- Right: (a) 3D view of anti‑Helmholtz coils (two coils with opposite currents) creating zero magnetic field at the center; six laser beams along x, y, z.  
- (b) Energy diagram: Zeeman effect (Energy vs. position), with magnetic sublevels \(m_J\) and circularly polarized beams \(\sigma^+\) and \(\sigma^-\) used to exert force.

Six laser beams along ±x, ±y, ±z, all circularly polarized. A magnetic field (via anti‑Helmholtz coils) is used to control the light pressure through the Zeeman effect.

---

## Exercises
1. Under what conditions does a material become superconducting, and why have we so far needed low‑temperature conditions?
2. If we want to make dry ice, what method do we use?
3. We want to see when argon gas solidifies. What can we do?
4. List ten applications of the Peltier effect.
5. Why do we first use liquid nitrogen (to reach 77 K) and then liquid helium to reach millikelvin temperatures?
6. What is superfluidity, and why does helium‑4 become superfluid at temperatures above 3 K?
7. Write about a recent scientific achievement attainable at low temperatures.
8. What can be done in physics with laser cooling?