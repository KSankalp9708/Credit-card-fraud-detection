# Credit Card Fraud Detection

---
## Objective
- To build and compare multiple machine learning models for **detecting fraudulent credit card transactions** using the **Kaggle** dataset

---
## Approach
- Data Preprocessing:
  - Imported and cleaned data using pandas and numpy.
  - Explored class distribution and performed stratified sampling to create a balanced subset.
- Model Training:
  - Implemented and trained the following models using scikit-learn:
    - Logistic Regression
    - Decision Tree
    - Random Forest
  - Tuned basic hyperparameters (max_depth, n_estimators, random_state, max_iter) for each model
- Evaluation:
  - Compared performance across models through **accuracy, F1-score, precision, and recall** evaluation *(see Results table)*
  
---
## Results
### Results  

| Model                | Accuracy (%) | F1 Score (%) | Precision (%) | Recall (%) |
|----------------------|-------------|-------------|--------------|-----------|
| **Logistic Regression**  | **94.42**       | **94.12**       | **98.88**        | 89.80     |
| Decision Tree        | 89.85       | 89.47       | 92.39        | 86.73     |
| Random Forest        | 92.89       | 92.47       | 97.73        | 87.76     |


**Key Observations**
- Logistic Regression achieved the *highest accuracy* **(94.4%)** and *strong precision–recall balance*, serving as a simple yet effective baseline.
- Random Forest performed competitively with *high precision* but slightly *lower recall*.
- Decision Tree offers interpretability, though with comparatively *lower metrics*.

---
## Conclusion
- This project demonstrates the use of multiple classification algorithms for binary fraud detection. Despite the dataset’s high original imbalance, resampling enabled fair model comparison. Logistic Regression stands out as a strong and efficient baseline for this dataset.
---
## Dataset
- The dataset is available on Kaggle:
- [Credit Card Fraud Detection Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- The dataset contains anonymized transaction features, a highly imbalanced target variable (fraud vs legit), and numeric attributes.
- A balanced subset was created with equal numbers of legitimate and fraudulent transactions (492 each) to ensure fair evaluation.
