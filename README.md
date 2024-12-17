# Car Price Prediction Using Machine Learning

## 📋 Project Description
This project aims to predict car prices using a dataset with multiple features like mileage, age, engine information, color, horsepower, and brand. The dataset is cleaned, preprocessed, and analyzed for insightful visualizations. A **Random Forest Regressor** model is implemented to predict car prices with a high degree of accuracy.

## 🛠 Features
1. **Data Cleaning and Feature Extraction**:
   - Extract fuel type, transmission type, color categorization, horsepower, and cylinder information.
   - Handle missing data effectively by imputing mean values for numerical features.

2. **Exploratory Data Analysis (EDA)**:
   - Hexbin plots, boxplots, pairplots, and heatmaps to analyze relationships and feature distributions.

3. **Data Encoding**:
   - Categorical features are encoded using **One-Hot Encoding** and **Ordinal Encoding**.

4. **Scaling**:
   - Data is standardized using **StandardScaler** to ensure uniform feature scaling.

5. **Model Training**:
   - Trained a **Random Forest Regressor** with an 84.15% R² score on the test set.

6. **Visualization**:
   - Compare predicted vs. actual values using scatter plots and diagonal benchmarks.

## 🚀 Technologies Used
- **Programming Language**: Python
- **Libraries**:
   - `pandas` - Data manipulation
   - `numpy` - Numerical operations
   - `seaborn` and `matplotlib` - Data visualization
   - `scikit-learn` - Machine learning (modeling and preprocessing)
   - `re` - Regular expressions for text parsing

## 📊 Data Preprocessing
### Key Functions:
1. **`extract_fuel_type`**:
   - Extracts fuel type from engine information.

2. **`extract_transmission_type`**:
   - Determines the transmission type.

3. **`categorize_color`**:
   - Groups exterior and interior colors into predefined categories.

4. **`extract_hp` and `extract_cylinders`**:
   - Parses engine details to extract horsepower and cylinder count.

### Handling Missing Data:
- Replaced null values in `price`, `horsepower`, and `Cylinders` with column means.

### Feature Engineering:
- Created additional features like car `age` using the latest model year.

## 📈 Model Performance
The **Random Forest Regressor** achieved:
- **RMSE (Root Mean Square Error):** 0.3871
- **R² Score:** 0.8415
