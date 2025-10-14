# Basic Electronic Components
## Resistors
A resistor resists the flow of electric current. It helps control voltage and current in a circuit.
### Ohm's Law:
V = I * R
#### Voltage = Current * Resistance
Measured in Ohms (Ω).
### Applications:
- Limiting current to an LED.
- Voltage dividers.
- Pull-Up and pull-down resistors in microcontrollers.
## Example: An LED Protected by a Resistor
- Without a resistor, components like LEDs would burn out instantly when connected to a power supply.
- That's why proper resistance calculation is critical.
### Use the color code to quickly determine resistor values!
## Capacitors
A capacitor stores electrical energy temporarily and releases it when needed.
#### Units: Farads (F)
### Basic Formula:
Q = C * V
#### Charge = Capacitance * Voltage
### Applications:
- Power supply filtering (smoothing ripple).
- Energy storage.
- Timing circuits (RC circuits).
## Diodes
- Allow current in one direction only.
- Block current in the opposite direction.
- Symbol: Arrow with a bar (|>) in circuit diagrams.
### Types of Diodes:
- Standard Diode: Protection against reverse polarity.
- Zener Diode: Voltage regulation.
- Light Emitting Diade (LED): Emits light.
## Transistors
### Types:
- BJT (Bipolar Junction Transistor) - current-controlled.
- MOSFET (Metal-Oxide-Semiconductor FET) - voltage-controlled.
### Three parts:
- Base (B)
- Collector (C)
- Emitter (E) - for BJT
#### (For MOSFETs: Gate, Drain, Source.)
### Main Functions:
- Switch: Turn circuits on / off electronically.
- Amplifier: Boost weak signals (used in radios, audio devices).
## Example
Lighting an LED through a resistor, controlled by a transistor acting as a swicth!
# Power Supply Design and Basics of PCB
## What is a Power Supply?
A power supply is an electrical device that provides the necessary voltage and current to your circuit.
- Convert: AC to DC (or change voltage levels)
- Regulate: Provide a stable output, even if input varies
- Filter: Remove noise and ripple
- Protect: Prevent overload, short circuit, etc.
## Types of Power Supply
Power supplies come in various flovors. Let's explore the main categories:
1. Linear Power Supplies
2. Switch Made Power Supplies (SMPS)
3. Battery Power Supplies
4. USB Power
## Linear Power Supplies
Use a transformer, rectifier, and  linear regulator like the famous 7805
- Simple and low noise
- But less efficient - because excess voltage is wasted as heat
## Switch Mode Power Supplies (SMPS)
- Use high-frequency switching to step down or up voltages.
- Examples: Buck, Boost, Buck-Boost converters
- Much more efficient
## Battery Power Supplies
- Use rechargeable or primary batteries.
- Often include battery management systems (BMS) for charging, protection, and voltage regulation.
## USB Power
- Widely used in IoT devices.
- Typically delivers 5V with current limits (500mA-3A depending on USB type)
## Components of Power Supply Design
1. Transformer (in AC-DC supplies)
2. Bridge Rectifier
3. Filter Capacitor
4. Voltage Regulator
5. Inductor (in SMPS)
6. Zener Diodes
7. Protection Devices
## Design Considerations
- Input and Output Voltage
- Load Current Range
- Efficiency Requirements
- Thermal Dissipation
- Size Constraints
- Cost and Availability
## Basics of PCB Design
A PCB is where your power supply and components physically sit. It connects them using copper traces instead of wires.
### Key layers:
#### Copper Layer:
For signal / power routing
#### Silkscreen:
Labels and component names
#### Soldermask:
The green coating that prevents shorts
## PCD Design Tools
KiCad, Eagle, EasyEDA, Altium Designer
## Basic Steps
- Schematic Design - Place and connect components logically.
- Component Placement - Arrange components physically on the board.
- Routing Traces - Connect the pins with appropriate width.
- DRC Check - Verify design rules before generating Gerber files.
- Export Gerber Files - used for manufacturing.
## Power Supply Layout in PCB
Power circuits need careful PCB layout to avoid heat, noise, and voltage drop.
### PCB Design Tips for Power Supplies:
- Thick Power Traces
- Short and Direct Paths
- Ground Planes
- Thermal Reliiefs
- Bypass capacitors
- Keep Feedback Traces Short
#### Good Layout = stable voltage and long component life.
