#  Bitcoin Money Laundering Detection using Machine Learning & Deep Learning

This project aims to classify Bitcoin transactions as either *legal* or *illegal* using a combination of machine learning and deep learning models. It is based on the Elliptic Dataset — one of the largest publicly available cryptocurrency transaction datasets.

>  **my project is part of a published research paper in IJACSA (2022)**  
> [ Click here to download the full research paper ](https://www.researchgate.net/publication/365119147_Money_Laundering_Detection_using_Machine_Learning_and_Deep_Learning)

---

##  Algorithms Used

This project evaluates the performance of the following classification models:

-  Random Forest (RF) – best performing
-  Deep Neural Network (DNN)
-  K-Nearest Neighbors (KNN)
-  Naive Bayes (NB)

---

##  Dataset

- **Name:** Elliptic Bitcoin Dataset  
- **Content:** 200K+ Bitcoin transactions across 49 graphs
- **Focus:** Only "legal" and "illegal" labeled transactions were used (46,564 transactions total)
- **Feature Selection:** Reduced from 166 features to 53 using correlation filtering and sklearn feature selection tools.

 [Dataset Source on Kaggle](https://www.kaggle.com/datasets/ellipticco/elliptic-data-set)

---

##  Results

Model performance was evaluated using F1-Score, Precision, Recall, and ROC-AUC:

| Model         | F1-Score | Precision | Recall | ROC-AUC |
|---------------|----------|-----------|--------|---------|
| **Random Forest** | **0.99** | 0.99      | 0.99   | 0.99    |
| DNN           | 0.98     | 0.98      | 0.98   | 0.97    |
| KNN           | 0.97     | 0.97      | 0.98   | 0.92    |
| Naive Bayes   | 0.74     | 0.99      | 0.59   | 0.90    |

 **Note:** Random Forest achieved the highest overall score due to its ability to handle imbalanced datasets.

---

##  Requirements

```bash
pip install -r requirements.txt
