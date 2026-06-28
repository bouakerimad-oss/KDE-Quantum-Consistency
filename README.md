# Mixture ZTP-G Framework for Bimodal QKD Data

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue)](https://www.python.org/)
[![License](https://img.shields.io/badge/License-MIT-green)](LICENSE)
[![arXiv](https://img.shields.io/badge/arXiv-2409.04746-red)](https://arxiv.org/abs/2409.04746)
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.14947231.svg)](https://doi.org/10.5281/zenodo.14947231)

## 📖 Overview

This repository contains the complete Python implementation of the **Mixture Zero-Truncated Poisson-Gamma (ZTP-G) model** developed for the analysis of bimodal Quantum Key Distribution (QKD) intensity data. The implementation includes:

- A numerically stable **Binned Expectation-Maximization (EM) algorithm**.
- **Soft-assignment classification** for empirical cluster validation.
- **Diagnostic metrics** for hardware characterisation: duty-cycle estimation, linearity calibration, and channel capacity computation.
- Full **reproducibility** of all figures and tables presented in the associated research paper.

The code is designed to be modular, well-documented, and easily adaptable to other optical communication datasets exhibiting multi-modal intensity distributions.

---

## ✨ Features

- **Robust Data Preprocessing** – Automatic extraction of measurement columns from raw QKD text files, removal of indices, zero suppression, and IQR-based outlier filtering.
- **Binned EM Algorithm** – Efficient parameter estimation for two-component Mixture ZTP-G models, scaling to millions of data points.
- **Numerical Stabilisation** – Data normalisation to prevent underflow when computing the ZTP-G density.
- **Diagnostic Suite**:
  - Duty-cycle estimation from mixing weights.
  - Linearity ratio $R = \mu_2 / \mu_1$ for amplifier calibration.
  - Channel capacity calculation from mixture entropy.
  - Proposed component-wise QBER decomposition framework.
- **Publication-Ready Visualisation** – Generation of histograms with overlaid mixture PDFs and individual components.

---

## 🚀 Installation

### Requirements

- Python 3.8 or higher
- Required packages are listed in `requirements.txt`.

### Clone and Install

```bash
git clone https://github.com/bouakerimad-oss/KDE-Quantum-Consistency.git
cd KDE-Quantum-Consistency
pip install -r requirements.txt
