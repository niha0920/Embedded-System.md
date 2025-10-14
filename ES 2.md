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
