# cirrhosis-survival-prediction

This project focuses on enhancing the prediction of survival outcomes for patients with cirrhosis using advanced machine learning techniques. It employs feature engineering, classification models, and optimization methods to improve predictive accuracy.

---

## **Overview**

Cirrhosis is a chronic liver condition with life-threatening consequences. This study utilizes the Mayo Clinic’s primary biliary cirrhosis dataset to predict patient survival states using logistic regression, support vector machines (SVM), and random forest algorithms. The project applies preprocessing, visualization, and tuning to compare and select the best-performing model.

---

## **Dataset**

- **Source**: Mayo Clinic study on primary biliary cirrhosis.
- **Features**:
  - Demographics: Age, sex.
  - Lab results: Bilirubin, albumin, and other liver function tests.
  - Clinical observations: Stage, edema, ascites.
- **Target Variable**: Survival state (`C`, `CL`, `D`).

---


## **Methods**

### **Data Preprocessing**
- Imputation for missing values (median for numeric, mode for categorical).
- One-hot encoding for categorical variables.
- Standardization of numeric features.
- Skewness correction using logarithmic and square root transformations.

### **Exploratory Data Analysis**
- Histograms and boxplots for distribution analysis.
- Correlation matrix and scatterplots for feature relationships.
- Outlier detection using Tukey’s method.

### **Modeling**
- **Algorithms**:
  - Multinomial Logistic Regression.
  - Support Vector Machines (SVM) with radial kernel.
  - Random Forest.
- **Optimization**:
  - Hyperparameter tuning (grid search, cross-validation).
  - Bagging to reduce variance.
  - Ensemble modeling with majority voting.

### **Evaluation**
- Metrics: Accuracy, Precision, Recall, F1-score, AUC.
- Validation: Holdout method and K-fold cross-validation.

---

## **Usage**

### **Requirements**
- R (>= 4.0)
- R Libraries: `caret`, `e1071`, `randomForest`, `ggplot2`, `dplyr`, `reshape2`, `pROC`, `ipred`, `glmnet`, `corrplot`, `psych`

### **Steps**
1. Clone the repository and place the `cirrhosis.csv` file in the `data/` directory.
2. Open `Cirrhosis_Survival_Prediction.Rmd` in RStudio.
3. Render the document to generate HTML, PDF, or Word reports.
4. View outputs in the `plots/` folder.

---

## **Results**

- **Best Model**: Random Forest achieved the highest accuracy and robustness.
- **Ensemble Model**: Improved performance using majority voting.
- **Insights**: Feature engineering and optimization significantly enhance model performance.

---

## **Future Directions**

1. Expand the dataset for greater generalizability.
2. Incorporate deep learning methods.
3. Utilize domain knowledge to refine feature selection.

---

## **Author**

- **Anusha Devi Doddi**  
  Graduate Student, Northeastern University  
  
---