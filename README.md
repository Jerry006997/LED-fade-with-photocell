# Arduino Photocell LED Fade (Non‑Blocking with millis)

This project demonstrates how to use a **photocell sensor** to control an LED that smoothly fades in and out when it’s dark. The sketch uses `millis()` for non‑blocking timing, avoiding `delay()` so the program stays responsive.

---

## ✨ Features
- LED fades up and down like a "breathing" effect.
- Photocell sensor detects ambient light.
- LED only pulses when it’s dark (sensor value above threshold).
- Uses `millis()` for timing — no blocking delays.
- Beginner‑friendly code with clear comments.

---

## 🛠 Hardware Required
- Arduino Uno (or compatible board)
- 1 LED (connected to PWM pin 9)
- 220Ω resistor for LED
- Photocell (LDR) sensor
- 10kΩ resistor (for voltage divider with photocell)
- Breadboard + jumper wires

---

## ⚡ Circuit Diagram
- **LED**:  
  - Anode → Pin 9 (PWM)  
  - Cathode → GND via 220Ω resistor  

- **Photocell**:  
  - One leg → 5V  
  - Other leg → A0 and → GND via 10kΩ resistor  

This forms a voltage divider so the photocell outputs a variable voltage to A0 depending on light level.
