**🏠 Property Price Predictor**
A simple machine learning project to predict property prices using location-based satellite images and basic property data.
This project focuses on data collection, preprocessing, and model experimentation rather than complex AI architectures.

**📌 Project Overview**

Real estate prices depend heavily on location and surroundings.
This project explores whether satellite images of a property’s location, along with structured property data, can help in predicting property prices.

The goal is learning and experimentation, not building a production-level system.

**📁 Project Structure**
Property_Price_Predictor/
│
├── map_fetcher.py
│   └── Fetches satellite images using latitude & longitude
│
├── preprocessing.ipynb
│   └── Cleans data and prepares features
│
├── model_training.ipynb
│   └── Trains and evaluates prediction models
│
├── 23117067_final.csv
│   └── Property dataset with labels
│
├── 23117067_report.pdf
│   └── Final project report
│
└── README.md

**📊 Dataset**

The dataset contains:

Property price (target variable)

Latitude & longitude

Other basic property-related features

Corresponding satellite images fetched from map APIs

Satellite images are retrieved based on the geographic coordinates of each property.

**🛰️ Satellite Image Collection**

map_fetcher.py is used to download satellite images using a map service API.

Steps:

Add your API access token inside map_fetcher.py

Run the script to download images for each property

Images are stored locally and referenced during training

python map_fetcher.py

🔧 Preprocessing

The preprocessing notebook performs:

Handling missing values

Feature selection

Scaling and normalization

Linking images to property records

Run:

preprocessing.ipynb

**📈 Model Training**

The training notebook focuses on:

Baseline regression models

Simple experiments with image features

Performance comparison using error metrics

Run:

model_training.ipynb


Evaluation uses standard regression metrics such as:

Mean Absolute Error (MAE)

Mean Squared Error (MSE)

R² Score

**🎯 Project Objective**

Understand how location imagery affects price prediction

Practice an end-to-end ML workflow

Gain experience working with real-world data issues

Combine structured data with external data sources

⚠️ Limitations

Small dataset

Satellite image quality depends on API source

Not optimized for real-world deployment

Results should be treated as experimental

🛠️ Technologies Used

Python

Pandas & NumPy

Scikit-learn

OpenCV

Jupyter Notebook

Map API (for satellite images)
