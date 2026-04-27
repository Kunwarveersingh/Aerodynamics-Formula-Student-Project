# Aerodynamics Formula Student - Project
# 🏎️ Formula Student — Aerodynamics Package

> Developing a full aerodynamics package for a Formula Student race car — from parametric CAD geometry to CFD-validated downforce targets.

---

## 📌 Project Overview

This repository documents the aerodynamics development process for a Formula Student car. The goal is to design, simulate, and iterate on a complete aero package — front wing, rear wing and undertray — to maximise downforce within competition regulations.

All design decisions, CFD results, and iteration history are tracked in a structured documentation system linked below.

---

## 📊 Project Tracker

All progress, CFD run logs, geometry versions, and targets vs actuals are tracked live in Google Sheets:

> 🔗 **https://docs.google.com/spreadsheets/d/1oe3-qxtIenzJk-B5498JtbZYvM2R236E6fPFWkVd6Y4/edit?usp=sharing**

---

## 🛠️ Tools & Workflow

| Stage | Tool |
|-------|------|
| Parametric CAD | Creo Parametric |
| CFD Simulation | Siemens StarCCM+ |
| Documentation | Google Docs / Google Sheets |
| Version tracking | GitHub |

### Workflow

```
CAD (Creo Parametric)
        │
        ▼
  Export geometry (STEP / STL)
        │
        ▼
  CFD Setup (StarCCM+)
  ├── Mesh generation
  ├── Physics: k-ω SST turbulence model
  └── Boundary conditions
        │
        ▼
  Post-process results
  ├── Extract Cl, Cd, L/D
  └── Pressure / velocity visualisations
        │
        ▼
  Log results → Google Sheets Run Log
        │
        ▼
  Iterate geometry
```

---

## 🏁 Aerodynamic Components

| Component | Status | Target Cl | Target Cd |
|-----------|--------|-----------|-----------|
| Front Wing | 🔄 In progress | TBC | TBC |
| Rear Wing | 🔄 In progress | TBC | TBC |
| Undertray | ⏳ Planned | TBC | TBC |
| Sidepods | ⏳ Planned | TBC | TBC |

> Targets are defined against Formula Student Germany (FSG) regulations.

---

## 📁 Repository Structure

```
fs-aero-package/
├── README.md
├── cfd/
│   ├── run_logs/          # CSV exports of each StarCCM+ run
│   ├── scripts/           # Python post-processing scripts
│   └── images/            # Pressure contours, streamlines, force plots
├── geometry/
│   └── exports/           # STEP / STL exports for CFD import
└── docs/
    ├── methodology.md     # CFD setup and mesh strategy
    └── results_summary.md # Key findings per iteration
```

> ⚠️ Raw Creo `.prt` files are not included — proprietary team IP. STEP exports are provided for reference geometry only.

---

## 📈 Key Results

*Results will be updated as iterations progress.*

| Iteration | Component | Cl | Cd | L/D | Notes |
|-----------|-----------|----|----|-----|-------|
| — | — | — | — | — | No results yet |

---

## 📷 CAD & CFD Visuals

> 🔗 **[CAD Design Visuals — Google Doc](YOUR_CAD_VISUALS_DOC_LINK_HERE)**

CFD images (pressure contours, streamlines, wake visualisations) will be added to `cfd/images/` as simulations progress.

---

## 🐍 Python Post-processing

Scripts in `cfd/scripts/` are used to:
- Parse StarCCM+ force reports (`.csv`)
- Plot Cl / Cd convergence over iterations
- Generate L/D comparison charts across geometry variants

---

## 🎓 University Project

This work forms part of an undergraduate **Mechanical Engineering** project. The full technical report and design log are maintained separately:

> 🔗 **[Design Log — Google Doc](YOUR_DESIGN_LOG_LINK_HERE)**
> 🔗 **[University Report — Google Doc](YOUR_REPORT_LINK_HERE)**

---

## 👤 Author

**Kunwarveer Singh**
Mechanical Engineering Student | Formula Student Aero Team Member

📬 Open to internship opportunities in motorsport & automotive engineering.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=flat&logo=linkedin)](YOUR_LINKEDIN_URL_HERE)

---

## 📄 License

Geometry exports and simulation scripts in this repository are shared for educational purposes. All rights reserved regarding original design IP.
