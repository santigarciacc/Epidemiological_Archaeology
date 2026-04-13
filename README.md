# 🏛️ Epidemiological Archaeology of SARS-CoV-2 (and Historical 1918 Benchmark)

![Python](https://img.shields.io/badge/python-3.8%2B-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Status](https://img.shields.io/badge/status-Under_Review-orange)

This repository contains the official codebase for the paper: **"Epidemiological Archaeology of SARS-CoV-2: Retrospective Inference of True Incidence via $H^3$ Topological Regularization of Excess Mortality"**.

It provides a scalable mathematical framework to retrospectively reconstruct the true infection and mortality curves of epidemics. By anchoring the analysis in high-fidelity excess mortality data, the model bypasses severe unobservability biases (testing shortages, reporting delays, political opacity) present in official institutional registries.

## 🚀 Key Features

* **$H^3$ Topological Regularization:** Smooths and filters noisy all-cause excess mortality data using Sobolev spaces to extract pure epidemiological signals with $C^2$ continuity.
* **Kinematic Time-Shift Operator:** Applies a robust clinical delay ($\tau$) from infection to death.
* **Dynamic IFR (Infection Fatality Ratio):** Adjusts lethality dynamically over time to account for viral mutations (e.g., Wild Type to Omicron) and population immunity/vaccination.
* **Global Scalability:** Automatically processes data for dozens of countries, calculating unobservability ratios for both infections and mortality.
* **Historical Zero-Testing Benchmark (1918 Influenza):** Validates the mathematical engine against the 1918 "Spanish Flu" pandemic, successfully reconstructing the Spring, Autumn, and Winter waves in a 100% unobservable environment across the US, UK, Spain, and British India.
* **Automated Visualizations:** Generates high-resolution, publication-ready 3-panel epidemiological dashboards and Error Evolution Audits (NMAE).

## 📊 Data Sources
This framework integrates modern and historical open datasets:

**SARS-CoV-2:**
1. [World Mortality Dataset (WMD)](https://github.com/akarlinsky/world_mortality) for all-cause mortality.
2. [JHU CSSE COVID-19 Data](https://github.com/CSSEGISandData/COVID-19) for official cases, deaths, and demographic baselines.

**1918 Influenza Benchmark:**
* Historical mortality scaling based on Taubenberger & Morens (2006), Chowell et al. (2008, 2014), and Chandra et al. (2012) for the United States, England & Wales, Spain (INE 1920), and British India.

## ⚙️ Installation

1. Clone the repository:
   ```bash
   git clone [https://github.com/TU_USUARIO/epidemiological-archaeology.git](https://github.com/TU_USUARIO/epidemiological-archaeology.git)
   cd epidemiological-archaeology

   pip install -r requirements.txt
pip install -r requirements.txt
