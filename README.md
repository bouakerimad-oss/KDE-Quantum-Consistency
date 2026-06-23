# KDE-Quantum-Consistency

**Numerical validation of almost sure uniform consistency of Kernel Density Estimation (KDE) on Schrödinger Cat states with quantum interference**

This repository contains the R code used in the paper:

> *"Almost sure uniform consistency of kernel density estimation for outcome densities induced by quantum measurements"*  
> Bouaker Imed (2023)

## 🔬 Overview

The code implements the theoretical framework of the paper, which proves that the KDE converges almost surely and uniformly on compact sets for densities arising from quantum measurements. The numerical simulation focuses on homodyne detection of a Schrödinger cat state, which includes a genuine quantum interference term with no classical analogue.

## 📊 Key Features

- **True density**: Schrödinger cat state with quantum interference term
  \[
  f(x) = \frac{1}{2}\mathcal{N}(-\mu) + \frac{1}{2}\mathcal{N}(+\mu) + \frac{1}{\sigma\sqrt{2\pi}} e^{-\mu^2/\sigma^2} \cos(2\mu x/\sigma^2)
  \]
- **KDE**: Epanechnikov kernel with Silverman's rule bandwidth \(h_n = 0.9\hat{\sigma}n^{-1/5}\)
- **Comparison**: Misspecified Gaussian MLE (fails to converge)
- **Statistics**: 100 Monte Carlo repetitions, sample sizes 200, 500, 1000, 2000
- **Metrics**: ISE, MAE, and \(L_\infty\) errors

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/YOUR_USERNAME/KDE-Quantum-Consistency.git
   cd KDE-Quantum-Consistency
