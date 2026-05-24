# DIGITAL-DEFENSE-ALGORITHM
The SYSTEM is an MIT-licensed R script that performs forensic screening on matrix datasets to detect data manipulation and fabrication. It works by analyzing pairwise sample numerical differences, generating warnings for potential copy-paste or data-scaling anomalies.
# ITAGAKI-SYSTEM: Digital Defense Algorithm (Numeric Forensics)

A high-performance numeric forensic utility developed in R to detect data fabrication, uncredited duplications, and artificial simulation patterns across multidimensional scientific or empirical datasets.

Developed by: **Tatsuki Itagaki**  
Copyright (c) 2026 Tatsuki Itagaki  
License: **MIT License**

---

## 📌 Overview

The **ITAGAKI-SYSTEM** performs raw numeric forensics by executing optimized pairwise comparisons across all samples (rows) in a dataset. It is specifically engineered to flag two primary indicators of data manipulation:

1. **Direct Fabrication (Copy-Paste):** Identifies rows that are 100% identical within a strict floating-point tolerance (`tol = 1e-9`).
2. **Proportional Scaling:** Identifies instances where data has been artificially simulated or manipulated via linear multipliers (scaling factors), characterized by a constant ratio across multi-component variables.

---

## 🛠️ Main Features

- **Automated Pairwise Comb**: Evaluates all combinations of sample pairings asynchronously via matrix operations.
- **Robust Multi-Type Input Handling**: Safely processes and standardizes `matrices`, `data.frames`, or nested numeric `lists`.
- **Comprehensive Logging**: Generates an external timestamped text report (`FORENSIC_NUMERIC_REPORT_YYYYMMDD_HHMMSS.txt`) documenting full analytical transparency.
- **Deep Dive Component Audit**: Isolates the exact raw values side-by-side for flagged pairs, mapping them to their corresponding metadata attributes.

---

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](https://opensource.org) page for legal details.
