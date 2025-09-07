# 🏡  Housing Price Prediction

## 📖 Project Overview
This project builds and evaluates machine learning models to predict California housing prices using the well-known housing dataset.  

The task includes:
- Data cleaning and preprocessing
- Exploratory Data Analysis (EDA) and visualization
- Feature engineering
- Model training and evaluation
- Comparison between different models

---

## 📂 Dataset
The dataset used is housing.csv, which contains information about California districts, including:
- Location (`longitude`, `latitude`)
- Demographics (`population`, households, `median_income`)
- Housing details (`total_rooms`, total_bedrooms, `housing_median_age`)
- Target: median_house_value

---

## ⚙️ Project Steps
1. Import libraries (pandas, numpy, matplotlib, scikit-learn, seaborn)
2. Upload and load data (`housing.csv`)
3. Data description & missing values (checked null values and handled them)
4. Data cleaning & feature engineering  
   - Imputed missing values in total_bedrooms  
   - Created new features (`rooms_per_household`, bedrooms_per_room, `population_per_household`)  
   - Applied log transformations for skewed features  
5. Exploratory Data Analysis (EDA)  
   - Histograms  
   - Scatter plots (e.g., median_income vs `median_house_value`)  
   - Geographic scatter plot (longitude vs latitude)  
   - Correlation heatmap  
6. Train/Test split (80/20)
7. Preprocessing pipeline using ColumnTransformer (numeric scaling, categorical encoding)
8. Model training  
   - Linear Regression (baseline)  
   - Random Forest Regressor  
9. Model evaluation  
   - Cross-validation with RMSE  
   - Final evaluation on test set  

---

## 📊 Results
- Linear Regression: Provided a simple baseline but with higher error.  
- Random Forest: Performed significantly better with lower RMSE.  
- The most important feature was median_income, strongly correlated with house value.  

---

## 🚀 Next Steps
- Hyperparameter tuning (GridSearchCV / RandomizedSearchCV for Random Forest).  
- Try more advanced models (Gradient Boosting, XGBoost, LightGBM).  
- Deploy the model as an API or web app.  

---

## 📝 Files in Repository
- California_Housing_Prediction.ipynb → Colab notebook with full code & explanations  
- housing.csv → Dataset  
- README.md → Project documentation  

---

## 👩‍💻 Author
This project was completed as part of a Machine Learning assignment.
