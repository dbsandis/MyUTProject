Here’s a **summary of the parts list** for the ultrasonic circuit shown in the schematic:

---

### **Major Components**
1. **Waveform Generator (CPLD)**
   - **Part**: CPLD (Complex Programmable Logic Device)  
     - Example: Xilinx XC9500 series or equivalent.
   - **Description**: Generates waveform signals (INA, INB, etc.) based on external inputs and clock source.

2. **Oscillator**
   - **Part**: 40 MHz Crystal Oscillator
   - **Description**: Provides a stable clock signal for the CPLD.

3. **High-Speed Logic Buffer**
   - **Part**: MD1812/MD1813  
   - **Description**: Buffers the CPLD signals to drive high-voltage pulsers.

4. **High-Voltage Pulsers**
   - **Part 1**: TC6320  
     - **Description**: Generates positive high-voltage pulses (up to +100V).
   - **Part 2**: TC2320  
     - **Description**: Generates negative high-voltage pulses (up to -100V).

5. **Ultrasonic Transducer**
   - **Part**: Ultrasonic transducer (e.g., 5 MHz piezoelectric transducer)
   - **Description**: Converts high-voltage pulses into ultrasonic waves.

---

### **Passive Components**
1. **Capacitors**
   - 0.22 µF (Decoupling for MD1812/13)
   - 0.47 µF (Decoupling for MD1812/13 and TC6320/TC2320)
   - 10 nF (Coupling capacitors for TC6320/TC2320)
   - 1 µF (Coupling capacitors for HVout to the transducer)

2. **Resistors**
   - Pull-down resistor for CPLD logic control (e.g., 10 kΩ).
   - Load resistor (RL) for transducer matching (value depends on transducer specifications).

3. **Diodes**
   - Schottky diodes for protection and signal rectification (if needed).

---

### **Miscellaneous**
1. **Jumper (JP)**
   - Configurable jumper for transducer coupling adjustments.

2. **LED Indicators**
   - LED1, LED2, LED3, and PWR for status and diagnostics.

3. **Power Supply**
   - **+10V and -10V** for the MD1812/13 and pulsers.
   - **3.3V or 5V** for CPLD logic.

4. **Connectors**
   - Pin headers or screw terminals for connecting the transducer and external controls.

---

### **Where to Source These Parts**
1. **CPLD, Pulsers (MD1812, TC6320/TC2320):**
   - Available from Mouser, Digi-Key, or Texas Instruments distributors.
2. **Oscillator, Capacitors, Resistors:**
   - Generic components available from Mouser, Digi-Key, or Amazon.
3. **Transducer:**
   - Ultrasonic transducers (e.g., 5 MHz) can be sourced from Olympus or specialized ultrasonic equipment retailers.

---

Would you like me to add estimated costs or a shopping list for these components? Let me know!

