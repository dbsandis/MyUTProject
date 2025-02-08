### **ADS127L01 Pinout and Raspberry Pi 5 Wiring Guide**
The **ADS127L01** is a high-speed **24-bit ADC** that supports **SPI and serial interfaces**. Below is the **pin mapping** and **how to wire it to the Raspberry Pi 5**.

---

## **📌 ADS127L01 Key Pinout**
| **Pin** | **Name** | **Function** | **Raspberry Pi 5 Connection (SPI Mode)** |
|---------|---------|------------|--------------------------------|
| 1 | **DVDD** | Digital Power (1.8V - 3.3V) | **3.3V (Pin 1)** |
| 2 | **DGND** | Digital Ground | **GND (Pin 6, 14, 20, etc.)** |
| 3 | **SCLK** | SPI Clock Input | **GPIO11 (Pin 23)** |
| 4 | **DIN** | SPI MOSI (Data In) | **GPIO10 (Pin 19)** |
| 5 | **DOUT** | SPI MISO (Data Out) | **GPIO9 (Pin 21)** |
| 6 | **CS** | Chip Select | **GPIO8 (Pin 24)** |
| 7 | **RESET** | Hardware Reset (Active Low) | **GPIO17 (Pin 11) (Optional)** |
| 8 | **PWDN** | Power Down (Active Low) | **Tie to HIGH for normal operation** |
| 9 | **FSYNC** | Frame Sync (for TDM mode) | **Tie to GND if not used** |
| 10 | **DRDY** | Data Ready (Interrupt) | **GPIO22 (Pin 15) (Optional)** |
| 11 | **AVDD** | Analog Power (3.3V - 5V) | **3.3V (Pin 1) or 5V (Pin 2)** |
| 12 | **AGND** | Analog Ground | **GND (Pin 6, 14, 20, etc.)** |

---

## **📌 Raspberry Pi 5 SPI Wiring to ADS127L01**
| **ADS127L01 Pin** | **Signal Name** | **Raspberry Pi 5 GPIO Pin** |
|-----------------|---------------|----------------------|
| 3  | **SCLK (Clock)** | **GPIO11 (Pin 23)** |
| 4  | **DIN (MOSI)** | **GPIO10 (Pin 19)** |
| 5  | **DOUT (MISO)** | **GPIO9 (Pin 21)** |
| 6  | **CS (Chip Select)** | **GPIO8 (Pin 24)** |
| 7  | **RESET (Optional)** | **GPIO17 (Pin 11)** |
| 10 | **DRDY (Interrupt)** | **GPIO22 (Pin 15)** |
| 1, 11 | **VDD (Power)** | **3.3V (Pin 1) or 5V (Pin 2)** |
| 2, 12 | **GND** | **GND (Pin 6, 14, 20, etc.)** |

---

### **🛠 Steps to Connect ADS127L01 to Raspberry Pi 5**
1. **Power the ADC:**
   - Connect **AVDD (Pin 11) and DVDD (Pin 1) → Raspberry Pi 3.3V (Pin 1)**
   - Connect **AGND (Pin 12) and DGND (Pin 2) → Raspberry Pi GND (Pin 6, 14, 20, etc.)**
   
2. **Connect SPI Data Lines:**
   - **SCLK (Pin 3) → GPIO11 (Pin 23)**
   - **DIN (Pin 4) → GPIO10 (Pin 19)**
   - **DOUT (Pin 5) → GPIO9 (Pin 21)**
   - **CS (Pin 6) → GPIO8 (Pin 24)**

3. **(Optional) Connect Additional Control Pins:**
   - **RESET (Pin 7) → GPIO17 (Pin 11)**
   - **DRDY (Pin 10) → GPIO22 (Pin 15)**

---

### **📌 Next Steps**
Would you like:
✅ **A KiCad schematic with this wiring?**  
✅ **Python code to test SPI communication with ADS127L01?**  

Let me know how I can assist! 🚀