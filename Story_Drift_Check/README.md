# Relative Story Drift Analysis 🏢📈

This module automates the checking of **Relative Story Drifts** directly from an active ETABS model to ensure structural performance under seismic loads.

## 📌 Compliance Check (TBDY 2018)
As per Section 4.9.1, the relative displacement ratio ($\Delta_i / h_i$) must be checked against code-defined limits (e.g., $0.008$ for RC structures) to prevent excessive damage to non-structural elements.

## ✨ Features
- **Automated Data Extraction:** Pulls drift ratios for all stories and directions (EX_RP, EY_RP).
- **Drift Profile Visualization:** Generates a vertical chart to visualize the building's deformation profile.
- **Batch Processing:** Checks multiple load cases simultaneously.

## 🚀 Usage
1. Open the ETABS model (analyzed state).
2. Run `relative_story_drifts.ipynb`.
