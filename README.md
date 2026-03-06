# Ultrapulse ⚡

Ultrapulse is a precision, web-based signal generator designed for high-frequency stochastic pulsing. Using the Web Audio API, it triggers sine wave bursts at millisecond intervals across ten distinct frequency groups, ranging from 1kHz to 40kHz.

## 🚀 Features

* **Ultra-Short Durations:** Precisely scheduled pulses between 1ms and 100ms.
* **Stochastic Frequency Hopping:** Random selection across mathematically defined frequency groups.
* **Safety First:** Default master volume set to `0.01` to protect hearing and hardware.
* **Live Visualizer:** Real-time oscilloscope to monitor impulse transients.
* **Detailed Logging:** Instantaneous readout of active frequency and source group.

## 🎛 Frequency Logic

The application cycles through 10 distinct groups with specific stepping patterns:
* **Group 1:** 1.0 kHz + 1.0 kHz steps (up to 40 kHz).
* **Group 2:** 1.5 kHz + 1.0 kHz steps (up to 39.5 kHz).
* **Groups 3-10:** Patterns starting from 1.1 kHz through 1.9 kHz in 1.0 kHz increments.

## 🛠 Usage

1.  Open `index.html` in any modern web browser.
2.  Adjust the **Master Volume** (Start low—high frequencies carry high energy).
3.  Set the **Pulse Duration** (1ms - 2ms for impulse testing).
4.  Click **INITIALIZE SEQUENCE**.

## ⚠️ Disclaimer

This tool generates frequencies up to 40kHz.
* **Nyquist Limit:** Most standard hardware (44.1/48kHz sample rates) cannot reproduce sounds above 22-24kHz.
* **Safety:** Prolonged exposure to high-frequency transients at high volumes can cause discomfort or damage to sensitive audio equipment.
