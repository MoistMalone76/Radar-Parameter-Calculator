# 📡 Radar & Comms Link Budget Calculator

An interactive, browser-based web application designed for RF engineers, defense analysts, and communications specialists to perform real-time radio frequency (RF) link budget analysis, radar range estimations, line-of-sight calculations, and OFDM throughput projections.

---

## 🚀 Features

The calculator is divided into six real-time RF engineering modules:

1. **Line of Sight & Target Kinematics**
   * Calculates Radar Horizon ($d_1$), Target Horizon ($d_2$), total Line of Sight (LOS) distance in kilometers and nautical miles, and intercept transit time based on Mach speed.
2. **Receiver Sensitivity**
   * Computes thermal noise floor ($k T B$), total receiver sensitivity, and required detection pulse bandwidth based on pulse width ($\tau$).
3. **Free Space Comms Link Budget**
   * Solves the Friis Transmission Equation with customizable inputs for Transmit Power ($P_t$), Antenna Gains ($G_t, G_r$), Frequency, Path Loss, and Receiver Sensitivity to compute output power ($P_t \text{ dBm}$), Received Power ($P_{rx}$), and overall **Link SNR**.
4. **Plane Earth Model (2-Ray Ground Reflection)**
   * Simulates $1/R^4$ propagation decay at low elevations considering antenna heights ($h_t, h_r$) and ground reflection effects.
5. **Radar Maximum Detection Range**
   * Solves the classic 4th-root Radar Range Equation including Pulse Integration ($N$), Radar Cross Section (RCS / $\sigma$), and Minimum Detectable Signal (MDS).
6. **OFDM Communications Data Throughput**
   * Estimates net digital throughput (Mbps) factoring in subcarriers, modulation code rates, overhead factor, and MIMO spatial multiplexing layers.

---

## 🛠️ Tech Stack

* **Frontend:** Single-page HTML5 + JavaScript (Vanilla ES6)
* **Styling:** [Tailwind CSS](https://tailwindcss.com/) (loaded via CDN)
* **Dependencies:** None (Zero build step or installation required)

---

## 📂 File Structure

```text
├── index.html       # Single self-contained HTML file containing UI & JS logic
└── README.md        # Project documentation
