# 🌾  Yield Predictor for Sri Lanka using Gradient Boosting Regressor

This project applies supervised machine learning techniques to predict agricultural yield in Sri Lanka based on historical crop data.  
It demonstrates a complete workflow — from data preprocessing and exploration to model training and evaluation — and is implemented fully in Python (Jupyter Notebook).

---

## Project Structure

Yield_Predictor/

├── Yield_Predictor.ipynb       # Main notebook with ML pipeline

├── sri_lanka_crop_data.csv     # Original dataset used for analysis

└── README.md                   # Project documentation



---

## Project Objective

The main objective of this project is to predict crop yield for Sri Lankan provinces and districts using available agricultural records.  
The dataset includes information such as crop type, province, district, cultivated area, production, and yield.  
The project demonstrates the use of Gradient Boosting Regression for accurate yield estimation.

---

## Dataset Description

**File:** `sri_lanka_crop_data.csv`

This dataset contains recorded information on agricultural production across various crops and regions in Sri Lanka.

### Main Columns

| Column | Description |
|:--------|:-------------|
| `Year` | Year of record |
| `Province` | Province in Sri Lanka (e.g., Central, Western, Southern) |
| `District` | District name |
| `Crop` | Name of the cultivated crop (e.g., Rice, Banana, Maize, Mango) |
| `Cultivated_Area` | Total cultivated area (acres)  |
| `Production` | Total production (kilograms) |
| `Yield` | Yield per acre (target variable) |


---

## Methodology

The notebook `Yield_Predictor.ipynb` follows a complete **machine learning regression workflow**:

1. **Data Loading**
   - Importing and viewing dataset  
   - Inspecting structure, missing values, and data types  

2. **Data Cleaning & Preparation**
   - Removing incomplete or invalid rows  
   - Converting data types and standardizing text labels  

3. **Exploratory Data Analysis (EDA)**
   - Visual summaries of yield by crop and province  
   - Relationship between cultivated area and production  
   - Bar charts and box plots for distribution analysis  

4. **Feature Encoding**
   - Label encoding for categorical attributes (`Province`, `District`, `Crop`)

5. **Model Development**
   - Splitting data into training and testing sets  
   - Training models:
     - **Gradient Boosting Regressor**

6. **Model Evaluation**
   - Metrics used:
     - **R² Score**
     - **Mean Absolute Error (MAE)**
     - **Root Mean Squared Error (RMSE)**
   - Visual comparison of predicted vs. actual yield values  

---

## Results Summary

| Model | R² Score | MAE | RMSE |
|:------|:---------|:----|:-----|
| Gradient Boosting Regressor | ~0.89 | Lower error | Best performance |


---

## Technologies Used

- **Python 3.x**
- **Pandas** – Data manipulation and cleaning  
- **NumPy** – Numerical computations  
- **Matplotlib / Seaborn** – Data visualization  
- **Scikit-learn** – Machine learning modeling and evaluation  

---

##  How to Run

1. **Clone the repository**
   ```bash
   git clone https://github.com/NadeeshaniKJ/yeild_predictor_for_sri_lanka_using_gradient_boosting_regressor.git
   cd Yield_Predictor
   ```

2. **Install dependencies**
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn
   ```

3.**Run the notebook**
   ```bash
   jupyter notebook Yield_Predictor.ipynb
   ```

Execute all cells sequentially to reproduce the analysis and model results.
