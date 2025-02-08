Yes, there are several **low-cost tools and services** available for creating your own PCB after prototyping and testing your DIY ultrasonic thickness measurement system. Here's a comprehensive guide:

---

### **1. PCB Design Tools (Free or Low-Cost)**

#### **a. KiCAD (Free and Open Source)**
- **Features**:
  - Professional-grade PCB design software.
  - Allows schematic capture and PCB layout for multi-layer designs.
  - Supports 3D rendering of your board.
- **Best For**: Complex designs with multiple components and custom footprints.
- **Website**: [KiCAD](https://www.kicad.org/)

#### **b. EasyEDA (Free/Online)**
- **Features**:
  - Browser-based tool for schematic and PCB design.
  - Integrated with LCSC for sourcing components and JLCPCB for manufacturing.
  - User-friendly for beginners with extensive libraries.
- **Best For**: Quick and simple designs, directly linked to low-cost PCB fabrication.
- **Website**: [EasyEDA](https://easyeda.com/)

#### **c. Fritzing (Low-Cost)**
- **Features**:
  - Simple, beginner-friendly interface for designing PCBs.
  - Good for basic layouts and hobbyist projects.
- **Cost**: ~$8 donation for the full version.
- **Best For**: Hobbyists or first-time PCB designers.
- **Website**: [Fritzing](https://fritzing.org/)

#### **d. Autodesk Eagle (Free for Students/Hobbyists)**
- **Features**:
  - Industry-standard PCB design software with extensive libraries.
  - Free version supports 2-layer designs up to 80 cm².
- **Best For**: Intermediate to advanced users looking for a robust design tool.
- **Website**: [Eagle](https://www.autodesk.com/products/eagle/overview)

---

### **2. PCB Fabrication Services (Affordable for Small Batches)**

#### **a. JLCPCB**
- **Features**:
  - Low-cost PCB fabrication, with prices starting at $2 for 5 PCBs (2-layer boards).
  - Supports high-quality manufacturing with silk-screening, solder mask, and various colors.
  - Direct integration with EasyEDA.
- **Best For**: Prototyping and small production runs.
- **Website**: [JLCPCB](https://jlcpcb.com/)

#### **b. PCBWay**
- **Features**:
  - Low-cost prototyping with options for 2–6 layer boards.
  - Includes assembly services for mounting components.
  - Prices start at $5 for 10 PCBs (100 mm x 100 mm boards).
- **Best For**: Boards requiring custom shapes or high precision.
- **Website**: [PCBWay](https://www.pcbway.com/)

#### **c. OSH Park**
- **Features**:
  - Small-batch PCB fabrication with a focus on high-quality manufacturing.
  - $5 per square inch for 3 PCBs, making it slightly pricier but great for high-end prototyping.
- **Best For**: U.S.-based small-scale developers and hobbyists.
- **Website**: [OSH Park](https://oshpark.com/)

#### **d. Seed Studio Fusion**
- **Features**:
  - Affordable PCB fabrication and assembly services.
  - Multiple finish options, including gold plating.
  - Prices start at $4.90 for 5 PCBs (100 mm x 100 mm boards).
- **Best For**: Prototyping and assembly in one place.
- **Website**: [Seeed Studio Fusion](https://www.seeedstudio.com/)

---

### **3. Tools for PCB Assembly (DIY Assembly at Home)**

#### **a. Soldering Tools**
- **Soldering Iron**:
  - Hakko FX-888D or Weller WE1010NA for precise soldering.
- **Solder Paste**:
  - Use solder paste and a stencil for SMD components.
- **Hot Air Rework Station**:
  - Essential for soldering and desoldering SMD parts (e.g., Quick 861DW).

#### **b. Stencils**
- **Purpose**:
  - Apply solder paste evenly for SMD components.
- **How to Get**:
  - Fabrication services like JLCPCB or PCBWay offer custom stencils at low cost.

#### **c. Pick-and-Place Tool (Optional)**
- Manual pick-and-place tools are affordable for home use:
  - e.g., **Neoden 4** for semi-automated assembly (for small production).

---

### **4. Prototyping PCBs In-House (DIY PCB Fabrication)**

If you want to fabricate PCBs yourself for testing, here are some methods:

#### **a. CNC PCB Milling**
- **What It Is**:
  - Use a small CNC machine to mill PCBs by removing copper.
- **Tools**:
  - **CNC Machines**: Snapmaker 2.0 or Genmitsu 3018-PRO.
  - **Software**: FlatCAM for generating G-code from PCB designs.
- **Best For**: Rapid prototyping of single-layer boards.

#### **b. Etching PCBs**
- **What It Is**:
  - Print the PCB layout onto a transparency sheet, transfer it to a copper board, and etch the unwanted copper.
- **Tools**:
  - Copper-clad board, etching solution (ferric chloride), and a laser printer.
- **Best For**: DIY prototyping with minimal investment.

---

### **5. Additional Tools for Testing and Validation**

#### **Oscilloscope**:
- Use a budget-friendly oscilloscope like **Rigol DS1054Z** for signal debugging and waveform analysis.

#### **Function Generator**:
- Generate high-frequency test signals using a device like the **Siglent SDG1032X** or **JDS6600**.

#### **Multimeter**:
- Measure resistance, continuity, and voltages during assembly and testing.

#### **Logic Analyzer**:
- Debug digital signals between your Raspberry Pi or Arduino and components (e.g., Saleae Logic Pro).

---

### **6. Recommended Workflow for Low-Cost PCB Production**

1. **Design**:
   - Use KiCAD, EasyEDA, or another tool to design your PCB, ensuring proper layout for your pulser, amplifier, and filters.

2. **Simulate**:
   - Simulate your circuit in LTspice or similar tools to verify its behavior.

3. **Fabricate**:
   - Upload your Gerber files to JLCPCB or PCBWay for fabrication.

4. **Assemble**:
   - Use solder paste and stencils for SMD components or solder manually.

5. **Test**:
   - Use an oscilloscope and multimeter to validate the circuit’s performance.

---

### **Next Steps**
- Let me know if you’d like help designing a PCB layout or creating Gerber files for your ultrasonic thickness measurement system.
- I can provide detailed steps or even design a simple PCB for your project using KiCAD or EasyEDA.