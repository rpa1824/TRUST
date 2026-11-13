# TRUST: Territory Resonance and Uncertainty-guided Stability Theory

## Overview

TRUST (Territory Resonance and Uncertainty-guided Stability Theory) is a territory-centric machine learning framework developed for breast cancer detection. The framework introduces a structured classification approach that models class-wise territorial occupation, feature resonance, territorial structures, absorption pathways, and prediction confidence.

Unlike conventional classification approaches that primarily rely on decision-boundary construction, TRUST characterizes the spatial organization of samples within the feature space and uses territorial relationships to perform classification.

## Framework Components

TRUST consists of six integrated modules:

1. **NOPD:** Numerical Occupation Pressure Detector
2. **TVEPD:** Territory Void Expansion and Pressure Dissolution
3. **TRSS:** Territory Resonance Stability Selection
4. **TFSB:** Territory Flux Structure Builder
5. **TAPE:** Territory Absorption Pathway Engine
6. **FCG:** Flux Confidence Generator

## Dataset

The framework is evaluated using the Wisconsin Diagnostic Breast Cancer (WDBC) dataset.

The classification task involves two diagnostic categories:
- Benign
- Malignant

## Implementation

The classifier is implemented in Python using NumPy, Pandas and Scikit-learn.

## Main Features

- Territory-based classification
- Class-wise occupation pressure analysis
- Territory-oriented sample generation
- Resonance-based feature selection
- Multi-center territorial modelling
- Territory absorption-based prediction
- Confidence score estimation
- Sample-level classification explanations

## Installation

Install the required dependencies:

```bash
pip install -r requirements.txt
```

## Usage

```python
from TRUST import TRUST

model = TRUST(
    sampling="auto",
    is_f=1,
    random_state=42
)

model.fit(X_train, y_train)

predictions = model.predict(X_test)

probabilities = model.predict_proba(X_test)

explanations = model.explain(X_test)
```

## Reproducibility

The implementation provides a fixed random-state option to support reproducible experiments. For rigorous evaluation, preprocessing, feature selection and sample generation should be performed using training data only.

## Research

This repository provides the implementation of the TRUST framework for academic research and reproducibility.

## Citation

Mohandas, L., Pramanik, M., & Panigrahi, R. (2026). A Territory Resonance and Uncertainty-guided Stability Theory (TRUST) for accurate breast cancer detection. Journal of King Saud University. Computer and Information Sciences, 38(9), 953.

## License

Refer to the LICENSE file for usage and redistribution terms.
