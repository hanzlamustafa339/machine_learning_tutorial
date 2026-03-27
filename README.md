# MLP Depth vs Width: A Tutorial Using Breast Cancer Data

[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

## Overview

This tutorial investigates how two key architectural hyperparameters — **depth** (number of hidden layers) and **width** (neurons per layer) — affect the performance of a Multilayer Perceptron (MLP) on the Breast Cancer Wisconsin dataset.

**Key findings:**
- Depth=4, Width=64 achieved the best test accuracy of **98.25%**
- Bigger networks do not always generalise better
- Feature scaling is essential for MLP training

## Files

| File | Description |
|------|-------------|
| `mlp_tutorial.ipynb` | Full Jupyter notebook with all code, experiments and figures |
| `mlp_tutorial.pdf` | PDF tutorial (<2000 words) |
| `README.md` | This file |
| `LICENSE` | MIT Licence |

## Getting Started

### Requirements
```bash
pip install scikit-learn matplotlib numpy pandas jupyter
```

### Run the notebook
```bash
jupyter notebook mlp_tutorial.ipynb
```

The notebook will download the Breast Cancer dataset automatically via `sklearn.datasets`.

## Dataset

**Breast Cancer Wisconsin (Diagnostic)**  
- 569 samples, 30 features, binary classification (malignant / benign)  
- Available via `sklearn.datasets.load_breast_cancer()`  
- Original paper: Street et al. (1993), SPIE Proceedings, 1905, 861–870

## References

- Goodfellow, I., Bengio, Y., & Courville, A. (2016). *Deep Learning*. MIT Press. https://www.deeplearningbook.org/
- Hornik, K. (1991). Approximation capabilities of multilayer feedforward networks. *Neural Networks*, 4(2), 251–257.
- Nielsen, M. (2015). *Neural Networks and Deep Learning*. http://neuralnetworksanddeeplearning.com/
- Pedregosa, F. et al. (2011). Scikit-learn: Machine Learning in Python. *JMLR*, 12, 2825–2830.
- Street, W. N. et al. (1993). Nuclear feature extraction for breast tumour diagnosis. *SPIE*, 1905, 861–870.

## Accessibility

- All figures use high-contrast colour palettes distinguishable without colour vision (shapes + line styles differentiate series)
- Alt-text descriptions are provided for all figures in the PDF tutorial
- Code is fully commented for screen reader users

## Licence

This project is licensed under the MIT Licence — see [LICENSE](LICENSE) for details.
