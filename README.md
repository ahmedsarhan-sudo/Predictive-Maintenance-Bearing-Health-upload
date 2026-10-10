# Predictive Maintenance: Bearing Fault Diagnosis

A machine learning project investigating bearing-health diagnosis
using vibration signals, signal processing, and deep learning.

## Objectives

- Explore and visualize vibration signals.
- Preprocess and segment time-series data.
- Analyze statistical and frequency-domain features.
- Develop CNN and LSTM classification models.
- Evaluate models using precision, recall, F1-score, and confusion matrices.

## Fault Classes

- Healthy bearing
- Inner race fault
- Outer race fault

## Project Structure

- `notebooks/` — data exploration and model experiments
- `data/` — local datasets, excluded from Git
- `src/` — reusable Python code
- `figures/` — project visualizations
- `results/` — evaluation outputs

## Dataset

The project uses bearing vibration data associated with the
Paderborn University bearing dataset.

Large datasets are excluded from version control. Dataset access
and preprocessing instructions will be documented separately.

## Getting Started

Create and activate a virtual environment:

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

Install dependencies:

```powershell
pip install -r requirements.txt
```

Launch Jupyter:

```powershell
jupyter notebook
```

Begin with `01_data_handling_visualization.ipynb`, followed by
the CNN and LSTM notebooks.

## Evaluation Integrity

Overlapping windows from the same recording should not be randomly
distributed across training and test sets. Group-aware splitting
helps reduce data leakage and overestimated performance.

## Author

Abdelrahman Mahmoud
