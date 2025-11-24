# 🔌 Day 1 — Breadboard & Power Basics

## 📘 Objectives
By the end of Day 1, you will be able to:

- Understand breadboard internal wiring  
- Safely use a DC bench power supply  
- Measure voltage, current, and resistance with a multimeter  
- Apply Ohm’s Law  
- Build your first LED circuit using the bench supply  

---

## 🧱 1. Breadboard Internal Wiring

A breadboard has two main areas:

### **Power Rails (Vertical)**
- Red rail = VCC  
- Blue/black rail = GND  
- Rails are connected vertically  
- Often split into upper and lower halves

-  🔴 (+): | | | | | | | | |
-  🔵 (−): | | | | | | | | |

### **Terminal Strips (Horizontal)**
Rows A–E are connected horizontally.  
Rows F–J are also connected horizontally.  
The middle gap separates the two halves, usually for ICs.

A B C D E----F G H I J

• • • • •----• • • • •

← row A–E----row F–J →

---

## 🔋 2. DC Bench Power Supply Basics

### Before powering anything:
1. Set voltage to **5.0V**  
2. Set current limit to **50–200mA**  
3. Keep output **OFF** when adjusting settings  

### Safety:
- Connect ground first  
- Never exceed 5V for basic LED circuits  
- Double-check wiring before enabling output  

---

## 🔧 3. Using a Multimeter

### **Voltage (V)**
- Set to DC Voltage  
- Red probe → VΩ  
- Black probe → COM  
- Measure across the component  

### **Current (A)**
⚠ Current must be measured **in series**.  
- Move red probe to **10A** port  
- Break the circuit  
- Insert meter inline  

### **Resistance (Ω)**
- Power off circuit  
- Measure resistor directly  

---

## 📐 4. Ohm’s Law

\[
V = I \times R
\]

For LED resistor sizing:

\[
R = \frac{V_{\text{supply}} - V_{\text{LED}}}{I_{\text{LED}}}
\]

Typical:
- Red LED drop ≈ 2.0V  
- Recommended LED current: 10–20 mA  

Example:

\[
R = \frac{5V - 2V}{0.02A} = 150Ω
\]

Use **150Ω–220Ω** safely.

---

## 🛠 5. Mini Project — Power an LED from the Bench Supply

### **Goal**
Power an LED using the bench supply while measuring voltage and current.

### **Materials**
- Breadboard  
- LED  
- 150–220Ω resistor  
- Bench power supply  
- Multimeter  
- Jumper wires  

### **Circuit Diagram**

                 +5V Supply
                     │
                     │
                ┌────┴────┐
                │ 150Ω    │   (Current-limiting resistor)
                └────┬────┘
                     │
                   ┌─┴─┐
                   │ > │   LED
                   └───┘
                     │
                    GND

### **Steps**
1. Place LED on breadboard  
   - Long leg (anode) → resistor → +5V  
   - Short leg (cathode) → GND  

2. Set power supply  
   - Voltage = **5.00V**  
   - Current limit = **50mA**  
   - Turn output ON  

3. Measure LED voltage  
   - Red LED: ~1.8 – 2.2V  
   - Blue/White: ~2.8 – 3.3V  

4. Measure current in series  
   - Expect 10–20mA  

5. Verify Ohm’s Law  
   - $ V_R = 5V - V_{LED} $  
   - $ I = \frac{V_R}{R} $

---

## 📸 Optional Photo
Add a picture of your circuit:

