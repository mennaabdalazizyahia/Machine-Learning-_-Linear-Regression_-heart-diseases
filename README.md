# ❤️ Heart Disease Prediction & Analysis

## 📖 Project Overview
This project focuses on analyzing and predicting **heart disease indicators** using the **Personal Key Indicators of Heart Disease dataset**.  
The workflow includes:
- Data cleaning and preprocessing
- Handling outliers
- Exploratory analysis
- Machine learning model training (Linear Regression)
- Model evaluation & saving for reuse

---

## 📂 Dataset
- **Source**: [Kaggle - Personal Key Indicators of Heart Disease](https://www.kaggle.com/datasets/cdc/heart-disease-indicators-dataset)  
- **Files Used**:  
  - `heart_2022_no_nans.csv` → Cleaned dataset without missing values  
- The dataset contains categorical and numerical health-related features such as BMI, smoking, alcohol use, physical activity, general health, and whether the patient had a heart attack.

---

## 🛠️ Tools & Libraries
- **Python** 🐍  
- **Pandas & NumPy** → Data manipulation & preprocessing  
- **Matplotlib & Seaborn** → Data visualization  
- **Scikit-learn** → Machine learning (Linear Regression, metrics, encoding)  
- **Joblib** → Model saving and loading  

---

## ⚙️ Steps Performed
1. **Load Dataset** from Kaggle input folder.  
2. **Data Cleaning**:
   - Checked missing values.  
   - Identified categorical & numerical features.  
   - Handled outliers using the **Interquartile Range (IQR)** method (replaced with median).  
3. **Exploratory Analysis**:
   - Displayed unique categorical values.  
   - Visualized relationships between features and `HadHeartAttack`.  
4. **Preprocessing**:
   - Label encoded the target variable (`HadHeartAttack`).  
   - Applied one-hot encoding to categorical features.  
5. **Model Training**:
   - Built a **Linear Regression** model to predict heart attack risk.  
   - Trained model on encoded features.  
6. **Model Evaluation**:
   - **Mean Absolute Error (MAE):** ~0.0836  
   - **Mean Squared Error (MSE):** ~0.0396  
   - Extracted model coefficients & intercept.  
7. **Model Saving**:
   - Saved trained model as `HeartDiseases` using Joblib.  
   - Reloaded model for future predictions.  

---

## 📊 Key Insights
- Outlier handling improved the dataset quality.  
- Several categorical health factors contribute to heart disease risk.  
- Linear Regression achieved **low error rates**, making it a potential baseline model.  

---

## 🚀 How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/mennaabdalazizyahia/heart-disease-analysis.git
   cd heart-disease-analysis
