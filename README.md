# ⭐ ATtiny85 Minimal System – Multilayer PCB Project

A compact multilayer PCB featuring the ATtiny85-20S microcontroller with proper power filtering, reset circuitry, and GPIO breakout.  
Designed as a learning-oriented embedded hardware project.

---

## 📌 **Objectives**

- Build a minimal, stable hardware setup for the ATtiny85 MCU  
- Learn multilayer PCB design flow  
- Implement proper decoupling and reset circuitry  
- Break out GPIO pins for programming & experimentation  
- Produce fabrication-ready Gerber & drill files  

---

## 🧩 **Project Overview**

This multilayer PCB includes everything required to run the ATtiny85 as a standalone microcontroller:

- ✔️ 5V Input  
- ✔️ Power filtering capacitors  
- ✔️ Reset switch + pull-up resistor  
- ✔️ GPIO/ISP header  
- ✔️ Stable multilayer routing  
- ✔️ Gerber + Drill + 3D View files included  

---

## 🔧 **Key Features**

- ATtiny85 in SOIC-8 package  
- Clean multilayer PCB layout  
- Professional schematic design  
- Proper decoupling (4.7µF + 0.1µF)  
- Reset control circuit  
- Compact and modular form factor  

---

## 🧠 **Working Principle**

### **1. Power Section**
- 5V input via header J1  
- C1 (4.7µF) → smooths low-frequency ripple  
- C2 (0.1µF) → handles fast switching noise  
- Ensures a clean and stable supply for the microcontroller

### **2. ATtiny85 Microcontroller (U1)**
- Operates on 5V  
- GPIO pins PB0–PB3 broken out via header J2  
- PB4 serves as Reset/I/O depending on configuration

### **3. Reset Circuit**
- R1 (10kΩ) keeps RESET pin pulled HIGH  
- SW1 pushes RESET LOW when pressed  
- Important for programming and debugging

### **4. GPIO / ISP Header**
Allows:
- ISP programming using USBasp / Arduino as ISP  
- Attaching sensors, LEDs, buttons, communication modules  
- General experimentation with ATtiny85 GPIOs  

---

## 🧰 **Applications**

This minimalist ATtiny85 board can be used for:

- Mini IoT nodes  
- Wearable electronics  
- LED drivers / light patterns  
- Sensor-based automation  
- Button-controlled gadgets  
- Low-power embedded systems  
- DIY hobby electronics  
- Educational microcontroller projects  

---

## 🧱 **Components Used**

| Component | Purpose |
|----------|---------|
| **ATtiny85-20S** | Main microcontroller |
| **C1 – 4.7µF** | Bulk decoupling |
| **C2 – 0.1µF** | High-frequency filtering |
| **R1 – 10kΩ** | Reset pull-up |
| **SW1** | Reset push button |
| **J1** | 5V power connector |
| **J2** | GPIO/ISP breakout header |

---
### 🛠 Tools Used
- KiCad 9.0 for schematic & PCB design   
- Gerber viewer for verification  

---

### 📚 Learnings
- Designing a minimal microcontroller hardware system  
- Power integrity: decoupling capacitors and filtering  
- Reset circuitry design (pull-up + switch)  
- Multilayer routing and stack-up basics  
- Creating fabrication files (Gerber + drill)  
- Schematic organization & PCB best practices
  
---

## 📁 **Repository Structure**

```
/Schematic  
    ATtiny85_Schematic.png

/PCB  
    Gerber_Files/  
    Drill_Files/  
    PCB_Layout.png  

/3D_View  
    PCB_3D_view.png  

README.md
```

---

## 🚀 **Future Enhancements**

- USB-C input  
- Onboard 5V/3.3V regulator  
- Power/status indicator LED  
- I²C expansion header  
- Bootloader support  

---

## ✍️ **Author**

**Niyathi Arun Kurthkoti**  
ECE Student | Aspiring Embedded & PCB Design Engineer
🔗 www.linkedin.com/in/niyathiarun
---


