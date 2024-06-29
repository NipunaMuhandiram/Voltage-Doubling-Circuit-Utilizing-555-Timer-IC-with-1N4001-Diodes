# Voltage Doubler Circuit using NE555 IC

This project demonstrates a voltage doubler circuit using the 555 Timer IC. The circuit steps up the input voltage to approximately double the input voltage.
## Project Description

This project demonstrates the construction of a voltage doubler circuit using a 555 Timer IC, 1N4001 diodes, and 1nF capacitors. The 555 Timer IC is configured in astable mode to generate a square wave, which is then used in conjunction with diodes and capacitors to double the input voltage.
## Components

- **IC**: 555 Timer
- **Diodes**: 2 x 1N4001
- **Capacitors**: 1 x 1nF, 2 x 1uF
- **Resistor**: 33KΩ

## PCB Design

![Circuit Diagram](https://github.com/NipunaMuhandiram/Voltage-Doubler-Circuit-using-NE555/blob/main/Snaps/1.png?raw=true)

## How It Works

The 555 Timer IC is configured in astable mode, generating a continuous square wave output. This output drives the charge pump circuit formed by the diodes and capacitors, effectively doubling the input voltage.

1. **555 Timer in Astable Mode**: The 555 Timer IC is configured in astable mode, meaning it produces a continuous square wave output. The frequency of this square wave is determined by the resistor and capacitors connected to it. In this circuit, the 33KΩ resistor and the capacitors set the oscillation frequency.

2. **Charge Circuit**: The output square wave from the 555 Timer drives the charge pump circuit, which consists of two diodes (1N4001) and two capacitors (1nF). The charge circuit operates in two phases:
   - **Phase 1**: When the output of the 555 Timer is high, the first capacitor charges through the first diode.
   - **Phase 2**: When the output of the 555 Timer is low, the charge from the first capacitor is transferred to the second capacitor through the second diode.

By continuously switching between these two phases, the voltage across the second capacitor is increased to approximately double the input voltage.

## Setup and Testing

1. **Assemble the Circuit**: Connect all the components as per the circuit diagram.
2. **Power the Circuit**: Provide an appropriate input voltage (e.g., 5V) to the circuit.
3. **Measure the Output**: Use a multimeter to measure the output voltage across the second capacitor. It should be approximately double the input voltage.

## Applications

This voltage doubler circuit can be used in applications where a higher voltage is required from a lower voltage source. Examples include:
- Powering devices that require a higher operating voltage
- Boosting battery voltage for certain applications
## Note

The actual output voltage may vary slightly due to the voltage drops across the diodes and the efficiency of the charge pump circuit.

## Acknowledgements

- Thanks to the open-source community for various resources and tutorials on voltage doubler circuits and the 555 Timer IC.
