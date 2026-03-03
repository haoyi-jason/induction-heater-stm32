# Circuit Design Documentation

## Circuit Explanation

The circuit design for the induction heater consists of several key components that work together to generate heat through electromagnetic induction. The main parts of the circuit include:

1. **Microcontroller**: The STM32 microcontroller controls the circuit by providing the necessary signals to drive the induction coil.
2. **Induction Coil**: This is the component that generates the magnetic field when an alternating current flows through it, which induces heat in the ferromagnetic material placed above it.
3. **Power Supply**: Provides the necessary voltage and current to the circuit components, particularly to the microcontroller and the induction coil.
4. **MOSFET Drivers**: These are used to switch the MOSFETs on and off, allowing the induction coil to be energized.
5. **Thermal Sensors**: These sensors measure the temperature of the heated object to ensure safe operating conditions.

## Component Details

- **STM32 Microcontroller**: 32-bit ARM Cortex-M microcontroller, typically STM32F103 series. It is equipped with timers, ADCs, and GPIOs for controlling the induction heating process.
- **Induction Coil**: Made of copper wire wound into a coil. The specifications should match the requirement for the expected induction heating application (number of turns, wire gauge, etc.).
- **Power Supply**: A DC power supply capable of providing necessary voltage (typically 12-24V) and current (up to 30A) depending on the design requirements.
- **MOSFETs**: N-channel MOSFETs rated for high power applications. Examples include IRF540 or similar, depending on the current requirements.
- **Thermal Sensors**: Such as LM35 or DS18B20 for temperature monitoring which can be interfaced with the STM32 for feedback control.

## Conclusion

This design allows for efficient heating of conductive materials through precisely controlled electromagnetic induction, making it suitable for various applications including cooking and metal working.