# 🏡 Property Price Predictor

**Property Price Predictor** is an advanced real-estate valuation framework that explores how satellite imagery can enhance house price prediction when combined with traditional structured data. This project integrates spatial visual context with tabular property features to build robust machine learning and deep learning models for more informed and accurate predictions.

---

## 📌 Project Overview

Real estate value depends on both property characteristics and neighbourhood context. While structured features like living area, location, and property grade strongly influence prices, visual signals from the surrounding area provide meaningful complementary information.

This repository implements and compares three predictive modeling strategies:

1. **Multimodal CNN + DNN Model**  
   - Combines satellite imagery processed by a Convolutional Neural Network (CNN) with structured features processed through a Deep Neural Network (DNN).  
   - Learns joint representations to capture both visual context and tabular information for price estimation.

2. **XGBoost on Tabular Data Only**  
   - Baseline XGBoost model trained exclusively on structured property features.  
   - Helps benchmark performance without image signals.

3. **XGBoost + Engineered Image Features**  
   - XGBoost model trained on tabular features enriched with engineered visual descriptors extracted from satellite imagery.  
   - Leverages visual cues like vegetation, built environment density, and neighbourhood layout.

Satellite imagery is collected via the **Mapbox Static API**, ensuring a standardized and consistent dataset of visual property context for all locations used in the study. :contentReference[oaicite:0]{index=0}

---

## 📁 Repository Structure


