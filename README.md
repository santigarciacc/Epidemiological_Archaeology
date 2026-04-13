# Epidemiological Archaeology: Mortality-Anchored Reconstruction of Epidemic Incidence

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)

This repository contains the data, source code, and Jupyter notebooks to reproduce the findings of the paper: **"Mortality-anchored reconstruction of latent epidemic incidence across COVID-19 and 1918 influenza: A retrospective 'Epidemiological Archaeology' study"**.

## Overview
During systemic crises such as the COVID-19 pandemic or the 1918 influenza pandemic, institutional case counts become unreliable due to diagnostic saturation or total lack of testing. This repository implements a novel mathematical framework that back-calculates the *true* latent incidence anchored entirely on all-cause excess mortality.

The core algorithm relies on a **Total Variation (TV) topological regularization within the $H^3$ Sobolev space**, filtering noise while preserving sudden structural breaks in transmission.

## Repository Structure
* `/src`: Contains the core Python modules:
  * `regularization.py`: Implementation of the $H^3$ TV penalty model.
  * `delay_kernels.py`: Infection-to-death discrete convolution operators.
  * `ifr_dynamics.py`: Time-varying Infection Fatality Ratio (IFR) functions.
* `/notebooks`: Step-by-step Jupyter notebooks reproducing the analyses for:
  * SARS-CoV-2 (COVID-19) global waves.
  * 1918 Influenza (USA, UK, and Spain).
* `/data`: Sample datasets (or links to full datasets like the World Mortality Dataset).

## Installation
To run the code, clone this repository and install the dependencies:

```bash
git clone [https://github.com/tu-usuario/Epidemiological-Archaeology.git](https://github.com/tu-usuario/Epidemiological-Archaeology.git)
cd Epidemiological-Archaeology
pip install -r requirements.txt
