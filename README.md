# Automated Essay Scoring - Kaggle Competition

This repository contains the solution for the Automated Essay Scoring Kaggle competition, where our team achieved a 0.8331 Cohen's Kappa score, ranking 409th out of 2708 contestants. We narrowly missed the bronze medal by just 0.001 in QWK score.

## Trained Models

### Individual Models
- **MyDeberta-v3-base**
  - OOF Score: 0.825
- **ChrisDeberta-v2-small**
  - OOF Score: 0.823

### Ensembles
- **CatBoost + LightGBM + XGBoost with DeBERTa OOF**
  - Weights: (0.3, 0.2, 0.5)
  - OOF Score: 0.839
- **CatBoost + LightGBM + XGBoost without DeBERTa OOF (500 Features)**
  - Weights: (0.25, 0.25, 0.5)
  - OOF Score: 0.829
- **Ensemble of MyDeberta-v3-base and ChrisDeberta-v2-small**
  - Weights: (0.5, 0.5)
  - OOF Score: 0.83
- **Final Ensemble Calculation**
  - Final ensemble = 0.8 * (0.7 * Ensemble 1 + 0.3 * Ensemble 2) + 0.2 * Ensemble 3

## Submission Summary

In total, we made around 150 submissions. Our final rank was 409 out of 2708 contestants. Despite our best efforts, we narrowly missed the bronze medal at the 270th rank by a 0.001 QWK score margin. However, one of our submissions scored higher at around 0.847.

---

Feel free to explore the code and approach used in this solution.
