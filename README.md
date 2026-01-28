# ETABS Base Shear Scaling Automation (TBDY 2018)

This project automates the **Base Shear Scaling** checks required by the Turkish Building Earthquake Code (TBDY 2018, Section 4.8.4) using Python and the ETABS API.

## 📌 Overview
In structural seismic design, dynamic analysis results ($V_{tB}$) must be compared against equivalent static base shear ($V_{tE}$). If $V_{tB} < 0.9V_{tE}$, analysis results must be scaled. This tool automates this repetitive process directly from an active ETABS model.

## ✨ Features
- **Real-time Connection:** Interacts with active ETABS models via Python.
- **Automated Calculations:** Computes scaling factors for both X and Y directions.
- **Professional Reporting:** Generates a clean summary table using `pandas`.
- **Regulatory Compliance:** Built for TBDY 2018 standards.

## 📊 Sample Output
The tool extracts data and provides a compliance status immediately:

| Direction | VtE (kN) | VtB (kN) | Limit (0.9*VtE) | Status | Scaling Factor |
|-----------|----------|----------|-----------------|--------|----------------|
| X         | 4179.34  | 413.43   | 3761.41         | ❌ INSUFFICIENT | 9.10 |
| Y         | 2954.82  | 336.21   | 2659.34         | ❌ INSUFFICIENT | 7.91 |

---
**Author:** Şeyda BAŞKAN
**Field:** Structural & Earthquake Engineering (M.Sc. Candidate)
