# Forest Cover Type Prediction

This project uses machine learning to predict forest cover type from cartographic variables in the [UCI Covertype Dataset](https://archive.ics.uci.edu/ml/datasets/covertype).  
It demonstrates **data preprocessing**, **class imbalance handling** with SMOTE, and **model training** using Decision Trees and Random Forests.

---

## 📂 Dataset
The dataset (`covtype.data`) contains cartographic variables such as:
- Elevation, Aspect, Slope
- Distances to hydrology, roadways, and fire points
- Hillshade values
- Wilderness areas and soil types (encoded as binary features)
- Cover Type (1–7) — the target variable

---

## 🛠 Workflow
1. **Data Loading & Cleaning**  
   - Assigns meaningful column names  
   - Checks for missing values and duplicates  
   - Descriptive statistics and basic EDA  

2. **Class Imbalance Handling**  
   - Uses **SMOTE** to oversample minority classes

3. **Model Training & Evaluation**  
   - **Decision Tree Classifier**  
   - **Random Forest Classifier**  
   - Metrics: Accuracy, Confusion Matrix, Classification Report

---

## 📊 Results
The Random Forest model outperforms the Decision Tree with higher accuracy and better class balance after SMOTE.

---

## 🚀 Requirements
  Install dependencies:
   
    ```bash
    pip install pandas matplotlib seaborn scikit-learn imbalanced-learn

  Run the notebook:
  
    jupyter notebook CoverType.ipynb
