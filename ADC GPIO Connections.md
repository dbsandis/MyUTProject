### **Which Raspberry Pi 5 GPIO Pin to Use for First Wire?**
Since you are interfacing a **high-speed ADC (ADS127L01) with Raspberry Pi 5** for ultrasonic testing, you should use **SPI or I2C GPIO pins** to communicate with the ADC.

---

### **1️⃣ SPI (Recommended for High-Speed ADC)**
SPI is faster than I2C and is recommended for **high-speed data transfer** from the ADC to the Raspberry Pi.

| **SPI Signal** | **Raspberry Pi 5 GPIO Pin** |
|--------------|--------------------|
| **SPI MOSI (Master Out, Slave In)** | GPIO10 (Pin 19) |
| **SPI MISO (Master In, Slave Out)** | GPIO9 (Pin 21) |
| **SPI SCLK (Clock)** | GPIO11 (Pin 23) |
| **SPI Chip Select 0 (CS0)** | GPIO8 (Pin 24) |
| **SPI Chip Select 1 (CS1)** | GPIO7 (Pin 26) |
| **GND (Ground)** | Pin 6, 14, 20, 25, 30, 34, 39 |
| **3.3V Power (For ADC logic level)** | Pin 1 |

👉 **First Wire Connection:**  
🔹 **GPIO10 (Pin 19) → ADC MOSI** (Master Out, Slave In)

---

### **2️⃣ I2C (If Your ADC Supports It)**
If your ADC uses **I2C instead of SPI**, use:

| **I2C Signal** | **Raspberry Pi 5 GPIO Pin** |
|--------------|--------------------|
| **I2C SDA (Data)** | GPIO2 (Pin 3) |
| **I2C SCL (Clock)** | GPIO3 (Pin 5) |
| **GND (Ground)** | Pin 6 |
| **3.3V Power (Logic level)** | Pin 1 |

👉 **First Wire Connection for I2C:**  
🔹 **GPIO2 (Pin 3) → ADC SDA (Data Line)**

---

### **📌 Which One Should You Use?**
✅ **Use SPI (GPIO10, GPIO9, GPIO11, GPIO8)** if the **ADC supports SPI**.  
✅ **Use I2C (GPIO2, GPIO3)** **only** if the ADC does not support SPI.

Would you like me to help with the **KiCad schematic wiring** for the Raspberry Pi 5 to ADC? 🚀