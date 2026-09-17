# ⚡ PIEX — Solar Plant Operations Dashboard

<div align="center">

![PIEX Dashboard](https://img.shields.io/badge/PIEX-Solar%20Operations-2563EB?style=for-the-badge&logo=sun&logoColor=white)
![Status](https://img.shields.io/badge/Status-Live%20Prototype-00BC7D?style=for-the-badge)
![Type](https://img.shields.io/badge/Type-UI%20Prototype-7C3AED?style=for-the-badge)

**A high-fidelity, interactive dashboard prototype designed for solar plant operators to monitor, analyze, and forecast energy production in real time.**

🌐 **[View Live Prototype →](https://souvik111.github.io/PIEX-dashboard-for-solar-plant-operators/)**

</div>

---

## 📸 Preview

| Screen | Description |
|---|---|
| **Dashboard** | Real-time KPIs, production charts, system alerts, and aerial plant monitoring |
| **Forecasting** | Production & irradiation forecast charts with weather-driven predictions |

---

## 🚀 Features

### 📊 Dashboard Screen
- **4 KPI Cards** — Current Power (7.54 MW), Total Daily Production (61.60 MWh), Today's Revenue (₺75,802), CO₂ Savings (10,986 kg) — each with trend indicators vs. the previous day
- **Production Analysis Chart** — Hourly-resolution area chart overlaying actual vs. expected production with interactive tooltip and annotated event markers
- **Statistical Summary Bar** — Peak Power (8.92 MW), Average Power (6.16 MW), Performance Ratio (82.6%), Capacity Factor (18.7%)
- **System Alerts Panel** — Real-time alert feed categorised as Critical / Warning / Normal with timestamps and severity icons
- **Solar Plant Monitoring** — Aerial satellite overlay showing per-inverter section output and efficiency (Sections A–D) with colour-coded health status
- **Section Performance Detail** — Glassmorphism overlay card for underperforming sections
- **Environmental Conditions** — Live weather tiles for Sunrise, Sunset, Temperature, Irradiation, and Rainfall

### 📈 Forecasting Screen
- **4 Forecast Stat Cards** — Predicted Daily Production (47.14 MWh), Maximum Irradiation (775 W/m²), Average Temperature (24.8 °C), Forecast Reliability (88%)
- **Production & Irradiation Forecast Chart** — Dual-axis overlay with confidence bands
- **AI Insight Banner** — Peak production window prediction

### 🧭 Navigation & Layout
- **Collapsible Sidebar** — Navigation links with alert badge counter + operator profile card
- **Top Bar** — Date picker and Hourly/Daily/Monthly time-range toggle
- **Multi-screen prototype routing** — Smooth screen transitions

---

## 🛠️ Technology Stack

| Layer | Technology |
|---|---|
| Markup | HTML5 |
| Styling | Inline CSS (pixel-perfect, Figma-exported) |
| Fonts | Inter via Google Fonts |
| Assets | SVG vector graphics + PNG images |
| Interactivity | Vanilla JavaScript |
| Hosting | GitHub Pages |

---

## 📂 Project Structure

`
piex/
├── index.html          # Single-file application (all screens + JS routing)
└── assets/             # 98 SVG/PNG assets exported from Figma
    ├── aerial.png      # Satellite photo overlay of the solar plant
    ├── avatar.png      # Operator profile avatar
    ├── group-*.svg     # Chart data visualisations & icon groups
    ├── frame-*.svg     # UI component frames
    ├── icon-*.svg      # Navigation & alert icons
    └── vector-*.svg    # Chart line & area vectors
`

---

## 🏃 Running Locally

`ash
# Clone the repository
git clone https://github.com/Souvik111/PIEX-dashboard-for-solar-plant-operators.git

# Navigate into the project
cd PIEX-dashboard-for-solar-plant-operators

# Open in your browser (Windows)
start index.html

# Or serve with any static server
npx serve .
`

---

## 🎨 Design System

| Token | Value |
|---|---|
| Primary accent | #2563EB (Blue 600) |
| Success / Online | #009966 (Green) |
| Warning / Degraded | #FB9600 (Amber) |
| Danger / Critical | #EB0000 (Red) |
| Revenue badge | #7C3AED (Violet) |
| Surface | #FFFFFF |
| Background | #F9FBFC |
| Text primary | #0F172B |
| Text secondary | #62748E |
| Card radius | 19px |

---

## 📐 Prototype Screens

| Screen ID | Name | Dimensions |
|---|---|---|
| s-dashboard | Operations Dashboard | 1440 × 1995 px |
| s-forecasting | Forecasting | 1440 × 1206 px |

The prototype auto-scales to fit any viewport via CSS 	ransform: scale().

---

## 🔮 Design Decisions

1. **Pixel-perfect Figma export** — HTML generated directly from Figma frames
2. **Glassmorphism detail panel** — Section performance card uses ackdrop-filter: blur(16px)
3. **Semantic alert severity** — Three-tier system with distinct icon sets and colour tokens
4. **Weather integration** — Environmental data contextualised with plant location (Konya, Turkey)
5. **Dual-axis forecast chart** — Production (MW) and irradiation (W/m²) on the same time axis

---

## 📄 License

Released for demonstration and portfolio purposes.
© 2026 PIEX — All rights reserved.

---

<div align="center">
Built with ☀️ for solar plant operators everywhere.
</div>
