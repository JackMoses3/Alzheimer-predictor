# Alzheimer’s Disease MRI Classification

## Project Overview

This project implements machine learning models to classify MRI scans into four stages of dementia:

- **Non-Demented**
- **Very Mild Dementia**
- **Mild Dementia**
- **Moderate Dementia**

Using MRI slice data, we compare **Convolutional Neural Networks (CNN)**, **Long Short-Term Memory Networks (LSTM)**, and a **hybrid CNN+LSTM** model to determine the most effective approach for early detection.

## Dataset

- **Source**: OASIS Alzheimer’s Detection Dataset ([Kaggle](https://www.kaggle.com/datasets/ninadaithal/imagesoasis/data))
- **Processing**:
  - MRI scans resized to **128x128 grayscale images**.
  - Data **balanced** to handle class imbalance issues.
  - Patients grouped for **spatial (CNN)** and **temporal (LSTM)** analysis.

## Models

1. **CNN**: Captures spatial patterns in individual MRI slices.
2. **LSTM**: Detects temporal patterns across multiple slices.
3. **CNN+LSTM**: Combines both approaches for improved classification.

## Results

- **CNN** achieved **99.16% accuracy**, making it the most practical model.
- **LSTM** showed instability due to limited data per patient.
- **CNN+LSTM** had potential but required more training data for reliability.

## Challenges & Learnings

- Addressing **class imbalance** for fair model evaluation.
- **Reducing overfitting** by adjusting dropout rates and layer configurations.
- Optimizing **training time** while maintaining accuracy.

## Usage

To run the model, execute the **Jupyter Notebook** provided.

---

**Contributors**: Raphael Schwalb, Max Fergie, Jack Moses  
**Course**: CPEN 355 - Group 1
