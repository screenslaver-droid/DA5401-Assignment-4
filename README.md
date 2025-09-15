# Assignment 4 – Classification and Model Evaluation submitted by CE22B106

This repository contains the code and analysis for **Assignment 4**, focusing on building and evaluating classification models.  
The notebook (`A4.ipynb`) demonstrates data preprocessing, model training, performance evaluation, and interpretation of results.  

---

##  Files
- `A4.ipynb` – Main Jupyter Notebook with all code, explanations, and outputs.
- `README.md` – Documentation and summary of the project.

---

##  Workflow Overview
1. **Data Loading & Exploration**
   - Import dataset and perform exploratory data analysis (EDA).
   - Check for missing values, data types, and distributions.

2. **Data Preprocessing**
   - Handle missing values and outliers.
   - Encode categorical variables.
   - Feature scaling/normalization.

3. **Model Training**
   - Logistic Regression as baseline.
   - Other models compared (e.g., Decision Tree, Random Forest, SVM, or Neural Net depending on notebook).
   - Hyperparameter tuning using grid search / cross-validation.

4. **Model Evaluation**
   - Accuracy, Precision, Recall, F1-Score.
   - ROC Curve and AUC.
   - Confusion Matrix interpretation.

5. **Cutoff Probability Analysis**
   - Default threshold = **0.5**.
   - Explore effect of varying cutoff probability.
   - Trade-offs between False Positives and False Negatives.
   - Optimal cutoff chosen using ROC/Youden’s J or F1 maximization.

6. **Results & Discussion**
   - Best performing model identified.
   - Key features influencing classification discussed.
   - Practical implications of cutoff adjustment explained.

---

##  Key Concepts
- **Cutoff Probability (Classification Threshold):**  
  Decides how probability predictions are mapped to class labels. Adjusting it can prioritize recall over precision (or vice versa), depending on the application.  

- **Evaluation Metrics:**  
  - **Accuracy**: Overall correctness.  
  - **Precision**: Fraction of predicted positives that are actually positive.  
  - **Recall (Sensitivity)**: Fraction of actual positives correctly identified.  
  - **F1-Score**: Balance between precision & recall.  
  - **ROC & AUC**: Trade-off between sensitivity and specificity.  

---

##  Requirements
Install the required Python libraries before running the notebook:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn
