# Crop Recommendation System

Recommends optimal crops to plant based on soil and climate parameters using machine learning.

## Overview

This project uses soil nutrients (N, P, K), temperature, humidity, pH, and rainfall to recommend the most suitable crop. It helps farmers make data-driven decisions for better yields.

## Dataset

- `crop recomend.csv` — Soil and climate parameters with corresponding crop labels

## Model

The system uses a trained classification model to predict the best crop. The pipeline includes:

- **Label Encoding** — Converts crop names to numerical values
- **MinMax Scaling** — Normalizes feature values
- **Classification Model** — Predicts the optimal crop

Saved artifacts:
- `crop_recomend_model.joblib` — Trained classifier
- `crop_recomend_label_encoder.joblib` — Label encoder
- `crop_recomend_minmax_scaler.joblib` — Feature scaler

## Requirements

- Python 3.8+
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- joblib

## Usage

1. Open the notebook:
   ```bash
   jupyter notebook "crop recomend.ipynb"
   ```
2. Run all cells to train the model and see predictions
3. Use the saved `.joblib` files to load the model for inference

## Results

- Provides crop recommendations based on input soil/climate parameters
- Visualizes feature distributions and model performance
