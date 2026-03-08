# NCS-API Website

> **NeuroCluster Streamer API — Interactive Web Interface & Demo Platform**

> **This project is under active development.** Features, simulations, and documentation are being added and refined continuously. Expect frequent updates.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Status](https://img.shields.io/badge/status-active%20development-orange.svg)]()
[![Netlify Status](https://api.netlify.com/api/v1/badges/your-site-id/deploy-status)](https://app.netlify.com/sites/your-site/deploys)

## About

The NCS-API Website is the front-end companion to the **NeuroCluster Streamer V8** clustering engine. It showcases the NCS algorithm through interactive, real-time simulations running entirely in the browser. The NCS algorithm performs streaming clustering with dynamic centroids, outlier scoring, and adaptive thresholds — ported to JavaScript for client-side demonstrations.

This is a **static website** — no build step, no Node.js required. Just HTML, CSS, and JavaScript served directly from Netlify.

## Live Demos

The website includes three interactive playground simulations, each powered by the NCS algorithm:

### 1. Interactive Clustering Playground
- 2D Canvas scatter plot with real-time point clustering
- Multiple algorithms: K-Means, DBSCAN, Hierarchical, and the proprietary NCS algorithm
- Visual membership lines, cluster halos, star-shaped centroid markers
- Outlier detection with scoring and visual indicators
- Adjustable parameters (cluster count, threshold, speed)

### 2. 3D Campus Network Security Simulation
- Three.js WebGL visualization of a university campus network
- Real-time threat detection and anomaly scoring via NCS
- Multiple scenarios: Normal traffic, DDoS attack, Ransomware, Data exfiltration, APT
- Kaspersky-style attack arcs, threat rings, and cable glow effects
- Interactive terminal selection with detailed info panels
- Building models with labeled departments and roaming devices

### 3. 3D Florida Weather Forecasting
- Three.js visualization of 24 real NOAA weather stations across Florida
- Accurate Florida state outline from GeoJSON coordinate data
- Weather scenarios: Normal, Hurricane, Cold Front, Heat Wave, Thunderstorm, Tropical Storm
- Real-time data layers: Temperature, Wind, Pressure, Precipitation
- Hurricane eye with rotating spiral arms, lightning effects, wind streaks, rain with wind drift
- NCS-powered anomaly detection across weather station data
- Station inspector with detailed meteorological readouts

## Tech Stack

| Technology | Usage |
|---|---|
| **HTML5 / CSS3 / Vanilla JS** | Core website — single `index.html` file |
| **Bootstrap 5.3.3** | Responsive layout, navigation, components |
| **Three.js r128** | 3D WebGL simulations (campus network, weather) |
| **Canvas 2D API** | Clustering playground scatter plots and charts |
| **Bootstrap Icons** | UI iconography |
| **Google Fonts (Inter)** | Typography |
| **Netlify** | Hosting and deployment |

No npm, no build tools, no bundler. Everything runs from a single HTML file with CDN dependencies.

## Project Structure

```
NeuroCluster-Streamer-Website/
├── NCS-API-welcome-page/
│   └── index.html              # The entire website (HTML + CSS + JS)
├── netlify.toml                # Netlify deployment config
└── README.md                   # This file
```

## Getting Started

### Run Locally

No dependencies to install. Just serve the static files:

```bash
# Clone the repo
git clone https://github.com/michaelkatsweb/NCS-API-welcome-page.git
cd NCS-API-welcome-page

# Serve with any static file server
python -m http.server 3000
# or
npx serve .
# or
php -S localhost:3000
```

Open `http://localhost:3000` in a modern browser (Chrome, Firefox, Edge, Safari).

### Deploy to Netlify

The site is configured for Netlify deployment. The `netlify.toml` sets the publish directory to `NCS-API-welcome-page/` with SPA-style redirects.

To deploy your own instance:
1. Fork or clone this repository
2. Connect it to Netlify
3. Netlify will auto-detect the config from `netlify.toml`
4. No build command needed — it's static files

## Design

- **Dark theme** with accent color `#7cc576`
- Background palette: `#0d0d1a`, `#1a1a2e`, `#16213e`
- Responsive design for desktop, tablet, and mobile
- Smooth CSS animations and transitions throughout

## Active Development Status

This project is **actively being developed**. Current and upcoming work includes:

### Recently Completed
- [x] Interactive 2D clustering playground with NCS algorithm
- [x] 3D campus network security simulation with threat detection
- [x] 3D Florida weather forecasting with real NOAA stations
- [x] Navigation dropdown for playground simulations
- [x] Netlify deployment pipeline

### In Progress
- [ ] API documentation page with live endpoint explorer
- [ ] Performance benchmarks and algorithm comparison charts
- [ ] Integration with the NCS-API FastAPI backend
- [ ] Additional clustering use-case examples

### Planned
- [ ] Real-time collaborative clustering sessions
- [ ] Additional 3D simulation scenarios
- [ ] Mobile-optimized simulation controls
- [ ] User data upload for custom clustering demos
- [ ] Multi-language code generation (Python, R, cURL)

## Part of the Heronix Ecosystem

This project is developed under **[Heronix Education Systems](https://heronixedu.com)** — a 2025 startup building on-premises school management software with a focus on data ownership and local control.

NCS-API serves as an R&D initiative within the Heronix ecosystem, exploring real-time clustering and anomaly detection techniques. The technology developed here feeds into Heronix's broader AI and analytics capabilities, including intelligent scheduling, pattern recognition in student data, and predictive analytics — all designed to run on-premises with zero cloud dependency.

### Related Projects

| Project | Description |
|---|---|
| **[Heronix Education Systems](https://heronixedu.com)** | On-premises school management platform (SIS, Scheduler, Messaging, Security) |
| **NCS-API-Project** | FastAPI backend powering the NeuroCluster Streamer API |
| **Heronix Scheduler V2** | AI-powered scheduling engine — a potential consumer of NCS clustering technology |

## Author

**Michael Katsaros** — Founder & CEO, Heronix Education Systems

Computer Science student at the University of the People. NCS started as a school project in 2024 — an experiment in streaming clustering algorithms that became a way to practice coding, explore data science, and build something real. It has since grown into an active R&D initiative within the Heronix ecosystem.

- GitHub: [@michaelkatsweb](https://github.com/michaelkatsweb)
- Website: [heronixedu.com](https://heronixedu.com)

## License

This project is licensed under the MIT License.

---

<div align="center">

**This project is under active development — contributions and feedback welcome!**

</div>
