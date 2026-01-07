
# 🏡 Property Price Predictor

**Property Price Predictor** is a multimodal real-estate price estimation project that studies the impact of satellite imagery when used alongside conventional tabular property data. The objective is to understand how visual neighbourhood information can complement structured features and contribute to more reliable and interpretable house price predictions.

---

## 📌 Project Overview

Property valuation is influenced not only by intrinsic attributes such as size, quality, and location, but also by the broader neighbourhood environment. While tabular features capture structural and locational aspects effectively, satellite imagery provides additional spatial context that is otherwise difficult to quantify.

This repository implements and evaluates three different modeling approaches to measure the contribution of visual information:

1. **Multimodal CNN + DNN Model**  
   - Satellite images are processed using a Convolutional Neural Network (CNN), while structured property attributes are handled through a Deep Neural Network (DNN).  
   - Feature representations from both networks are fused to predict house prices in an end-to-end multimodal setup.

2. **XGBoost with Tabular Data Only**  
   - A baseline XGBoost model trained exclusively on structured real-estate features.  
   - Serves as a benchmark to assess the predictive power of traditional data without visual inputs.

3. **XGBoost with Tabular and Image-Derived Features**  
   - XGBoost trained on tabular data augmented with engineered features extracted from satellite imagery.  
   - Enables the model to incorporate neighbourhood-level visual cues such as greenery, built density, and spatial layout.

Satellite images are obtained using the **Mapbox Static API**, ensuring a consistent and standardized overhead view of each property’s surrounding area across the dataset.

---

## 📁 Repository Structure



├── Final csv file.csv        # Final processed dataset
├── Map_Fetcher.py            # Script to fetch satellite images using Mapbox API
├── Preprocessing.ipynb      # Data cleaning, feature engineering, and preprocessing
├── Model_Training.ipynb     # Model training, evaluation, and comparison
├── README.md                # Project documentation


---

## ⚙️ Setup & Requirements

To run this project, ensure the following requirements are met:

- Python 3.x  
- pandas, numpy, scikit-learn  
- xgboost  
- tensorflow / keras  
- Mapbox API access token  

---

## 🚀 How to Run

1. Clone the repository:
  
   git clone https://github.com/lalitjingar90/Property_Price_Predictor.git


2. Use `Map_Fetcher.py` to download satellite images for each property location.
3. Run `Preprocessing.ipynb` to clean the dataset and generate features.
4. Execute `Model_Training.ipynb` to train models and evaluate their performance.

---

## 📊 Evaluation Metrics

Model performance is assessed using standard regression metrics:

* **RMSE (Root Mean Squared Error)**
* **MAE (Mean Absolute Error)**
* **R² (Coefficient of Determination)**

---

## 📈 Key Findings

* Structured tabular features such as living area, property grade, and location account for most of the predictive power.
* Satellite imagery captures meaningful neighbourhood-level characteristics that correlate with property prices.
* Visual features provide complementary context, improving model interpretability and robustness.
* Multimodal learning enhances understanding of spatial effects in real-estate valuation rather than replacing traditional features.

---

## 🧠 Conclusion

The results demonstrate that satellite imagery contains economically relevant information and can effectively augment traditional house price prediction models when integrated with structured real-estate data. This project highlights the potential of multimodal approaches for building more holistic and explainable real-estate valuation systems.

---

## 📄 License

This project is open-source and intended for academic and educational use.

