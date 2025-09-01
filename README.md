# Credit Card Fraud Detection

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]([https://github.com/KSankalp9708/Credit-card-fraud-detection/blob/main/Credit_card_fraud_detection.ipynb])

---
## Objective
- To build and compare multiple machine learning models for **detecting fraudulent credit card transactions** using the Kaggle dataset

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
  - Compared performance across models through accuracy evaluation *(see Results table)*
  
---
## Results
| Model               | Accuracy (%) |
| ------------------- | ------------ |
| Logistic Regression | **93.40**    |
| Decision Tree       | 91.88        |
| Random Forest       | 92.89        |

**Key Observations**
- Logistic Regression achieved the **highest accuracy (93.4%)** and serves as a simple yet effective baseline.
- Ensemble methods (Random Forest) performed competitively but with slightly *lower accuracy* on this balanced subset.
- Decision Tree offers interpretability, though slightly *less accurate*.

---
## Conclusion
- This project demonstrates the use of multiple classification algorithms for binary fraud detection. Despite the dataset’s high original imbalance, resampling enabled fair model comparison. Logistic Regression stands out as a strong baseline for this dataset.
---
## Dataset
- The dataset is available on Kaggle:
- [Credit Card Fraud Detection Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- The dataset contains anonymized transaction features, a highly imbalanced target variable (fraud vs legit), and numeric attributes.
- A balanced subset was created with equal numbers of legitimate and fraudulent transactions (492 each) to ensure fair evaluation.
