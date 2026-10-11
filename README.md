# quantum-split

> A high-precision, real-time gratuity engine and bill-splitting web application designed with a sleek, high-tech interface and adaptive rounding controls.

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
* **Live Reactive Math**: Instantly updates all metrics on every keystroke or slider interaction.
* **Dual Breakdown**: Displays both combined totals (Base Bill, Tip Total, Grand Total) and individual shares (Per-Person Bill, Per-Person Tip, Per-Person Total).
* **Effective Tip Auditing**: Dynamically calculates and displays the true tip percentage after any rounding adjustments are applied.

### 🎛️ Adaptive Tip Controls
* **Quick Presets**: Instant selection chips for `10%` (Standard), `15%` (Good), `18%` (Great), `20%` (Generous), and `25%` (Superior).
* **Fine-Tuning Slider**: Smooth responsive slider ranging from `0%` to `50%`.
* **Direct Numeric Input**: Supports exact custom percentages from `0%` to `100%`.
* **Quick Bill Preset Chips**: Rapidly test or set bill amounts (`$25`, `$50`, `$75`, `$100`, `$150`, `$200`).

### 👥 Dynamic Party Splitting
* **Flexible Group Sizing**: Split bills seamlessly across 1 to 100 people using interactive steppers (`−` / `+`), a range slider, or direct numeric entry.
* **Party Size Visualizer**: Glowing cybernetic avatar dots provide immediate visual confirmation of party count.
* **Individual Shares Roster**: Expandable breakdown drawer detailing the exact charge assigned to each person in the group.

### 📐 Precision & Rounding Logic
Choose between three distinct calculation modes to fit any dining scenario:
1. **Exact Cents (Default Precision)**: Calculates down to the penny with exact mathematical accuracy.
2. **Round Up / Person (Clean Split)**: Rounds each individual's portion up to the nearest whole dollar—ideal for avoiding loose change or split credit card transactions.
3. **Round Up Total (Cash Friendly)**: Rounds the entire combined bill up to the nearest whole dollar while keeping splits proportional.
4. **Rounding Delta Tag**: Automatically displays a live badge indicating the exact extra cents contributed to the tip due to rounding.

### 🌍 Multi-Currency & Utility
* **Global Currency Selector**: Toggle between USD (`$`), EUR (`€`), GBP (`£`), JPY (`¥`), CAD (`CA$`), AUD (`A$`), and CHF (`CHF`).
* **One-Click Receipt Export**: Copy a clean, formatted ASCII text receipt breakdown directly to the clipboard with animated toast confirmation.
* **Zero External Dependencies**: 100% self-contained vanilla HTML5, CSS3, and JavaScript—zero build steps, zero `node_modules`, and works completely offline.

---

## 🛠️ Tech Stack & Architecture

* **Frontend**: Vanilla HTML5, CSS3, JavaScript (ES6+)
* **Styling**:
  * CSS Custom Properties (Theming)
  * Glassmorphism (`backdrop-filter: blur(20px)`)
  * Cybernetic obsidian & neon palette (`#00f0ff` cyan, `#10b981` emerald, `#0f172a` slate)
  * Tabular monospace typography for numeric alignment
  * Fully responsive CSS Grid & Flexbox layouts (desktop & mobile optimized)
* **Icons**: Inline scalable SVGs (no external icon fonts or CDN requests required)

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
├── index.html           # Main application entry point (single-file bundle)
├── tip_calculator.html  # Standalone backup application bundle
├── style.css            # Modular stylesheet
├── script.js            # Modular reactive logic
└── README.md            # Project documentation and deployment guide
```

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).
