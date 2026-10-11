# quantum-split

> A high-precision, real-time gratuity engine and bill-splitting web application designed with a sleek, high-tech interface, dedicated modular settings, and adaptive rounding controls.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![GitHub Pages](https://img.shields.io/badge/Deployment-GitHub%20Pages-00f0ff.svg)](#-live-web-application)
[![Dependencies](https://img.shields.io/badge/Dependencies-Zero%20(Vanilla)-10b981.svg)](#-tech-stack--architecture)
[![Platform](https://img.shields.io/badge/Platform-Web%20%2F%20Mobile-38bdf8.svg)](#-key-features)

---

## 🌐 Live Web Application

Access the live web application hosted on GitHub Pages:

👉 **[https://yusuke614.github.io/quantum-split/](https://yusuke614.github.io/quantum-split/)**

---

## ✨ Key Features

### ⚡ Real-Time Gratuity & Bill Telemetry
* **Live Reactive Math**: Instantly updates all metrics on every keystroke, slider drag, or stepper click.
* **Dual Breakdown**: Displays both combined totals (Base Bill, Tip Total, Grand Total) and individual shares (Per-Person Bill, Per-Person Tip, Per-Person Total).
* **Effective Tip Auditing**: Dynamically calculates and displays the true tip percentage after any rounding adjustments are applied.

### 🎛️ Adaptive Tip Controls
* **Quick Presets**: Instant selection chips for `10%` (Standard), `15%` (Good), `18%` (Great), `20%` (Generous), and `25%` (Superior).
* **Dual Stepper Controls (`−` / `+`)**: Increment or decrement tip percentages in crisp 1% steps.
* **Fine-Tuning Slider**: Smooth responsive slider ranging from `0%` to `50%`.
* **Direct Numeric Input**: Supports exact custom percentages from `0%` to `100%`.
* **Quick Bill Preset Chips**: Rapidly test or set bill amounts (`$25`, `$50`, `$75`, `$100`, `$150`, `$200`).

### 👥 Dynamic Party Splitting
* **Flexible Group Sizing**: Split bills seamlessly across 1 to 100 people using interactive steppers (`−` / `+`), a range slider, or direct numeric entry.
* **Party Size Visualizer**: Glowing cybernetic avatar dots provide immediate visual confirmation of party count.
* **Individual Shares Roster**: Expandable breakdown drawer detailing the exact charge assigned to each person in the group.

### ⚙️ Dedicated Settings & Configuration Tab
A streamlined tab navigation separates real-time calculation from preference configuration:
1. **Precision & Rounding Logic**:
   * **Exact Cents (Default Precision)**: Calculates down to the penny with exact mathematical accuracy.
   * **Round Up / Person (Clean Split)**: Rounds each individual's portion up to the nearest whole dollar—ideal for split credit card transactions.
   * **Round Up Total (Cash Friendly)**: Rounds the entire combined bill up to the nearest whole dollar while keeping splits proportional.
   * **Live Rounding Delta Tag**: Highlights the exact extra cents contributed to the tip due to rounding.
2. **Session Persistence**:
   * Automatically remembers your selected **Tip Calculation & Rounding Mode**, currency denomination, and theme across browsing sessions via safe client-side `localStorage`.
3. **Global Currency Configuration**:
   * Instantly switch between USD (`$`), EUR (`€`), GBP (`£`), JPY (`¥`), CAD (`CA$`), AUD (`A$`), and CHF (`CHF`).
4. **Receipt & Export Preferences**:
   * Toggle inclusion of the full itemized individual roster in the clipboard export.
   * Toggle inclusion of the rounding audit breakdown in the clipboard export.
5. **Holographic Themes & Audio Telemetry**:
   * Four dynamic accent palettes: **Cyber Cyan** (`#00f0ff`), **Matrix Emerald** (`#10b981`), **Solar Amber** (`#f59e0b`), and **Void Violet** (`#a855f7`).
   * Web Audio API sound effects toggle providing synthesized high-tech micro-feedback during interactions.
6. **One-Click Defaults Restore**:
   * Dedicated reset button inside settings to restore all calculation and UI preferences to default.

---

## 🛠️ Tech Stack & Architecture

* **Frontend**: Vanilla HTML5, CSS3, JavaScript (ES6+)
* **Storage**: Client-side `localStorage` with `safeStorage` wrapper (sandboxed and `file://` resilient)
* **Styling**:
  * CSS Custom Properties (Dynamic Theming)
  * Glassmorphism (`backdrop-filter: blur(20px)`)
  * Cybernetic obsidian & multi-accent glow palettes
  * Tabular monospace typography for numeric alignment
  * Fully responsive CSS Grid & Flexbox layouts (desktop & mobile optimized)
* **Audio**: Native Web Audio API (`AudioContext`, `OscillatorNode`) with zero external sound files.
* **Icons**: Inline scalable SVGs (no external icon fonts or CDN requests required).

---

## 🚀 Quick Start & Deployment

### Running Locally

No installation or build tools required. Simply clone the repository and open `index.html`:

```bash
# Clone the repository
git clone https://github.com/yusuke614/quantum-split.git

# Navigate into the project folder
cd quantum-split

# Open directly in your browser
open index.html

# Or start a lightweight local web server
python3 -m http.server 8000
```
Then visit `http://localhost:8000` in your web browser.

---

### Deploying to GitHub Pages

1. **Create Repository**:
   * Create a new public repository on GitHub named **`quantum-split`**.
2. **Push Files**:
   * Ensure `index.html` (the primary application entry point) is committed to the `main` branch:
   ```bash
   git init
   git add .
   git commit -m "Initial commit: Quantum Split gratuity engine"
   git branch -M main
   git remote add origin https://github.com/yusuke614/quantum-split.git
   git push -u origin main
   ```
3. **Enable GitHub Pages**:
   * Go to your repository on GitHub.
   * Click **Settings** → **Pages** (under "Code and automation" in the left sidebar).
   * Under **Build and deployment** → **Source**, select **Deploy from a branch**.
   * Under **Branch**, choose **`main`** and folder **`/ (root)`**, then click **Save**.
4. **Access Your Live Web Application**:
   * Within 1–2 minutes, your application will be live at:
     ```
     https://yusuke614.github.io/quantum-split/
     ```

---

## 📂 Repository Structure

```text
quantum-split/
├── index.html           # Main application entry point (v4 with session persistence)
├── tip_calculator.html  # Standalone application bundle (v4 with session persistence)
├── style.css            # Modular stylesheet
├── script.js            # Modular reactive logic
└── README.md            # Project documentation and deployment guide
```

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).
