# Telecom Customer Churn Prediction

> Exploring customer segments with k-means clustering and predicting churn with a random forest classifier.

---

## Overview

This project examines telecom customer data through two complementary analyses. The first notebook uses k-means clustering to explore customer segments. The second trains and evaluates a random forest classifier to predict customer churn.

Together, the analyses explore patterns in customer behavior and assess how well a supervised model can distinguish customers who churn from those who do not.

---

## Business Problem

Customer churn can reduce revenue and increase the need to acquire replacement customers. Understanding differences among customers and identifying those at higher risk of leaving could help a telecom business focus its retention efforts.

Clustering explores whether the available customer characteristics form useful groups. Churn classification addresses a different question: how accurately can those characteristics help predict a known outcome?

---

## Objectives

- Prepare customer data for clustering and classification
- Use k-means to explore customer segments
- Train a random forest model to predict churn
- Evaluate clustering quality and predictive performance
- Interpret the results and their practical limitations

---

## Technologies Used

| Category | Technologies |
|---|---|
| Language | Python |
| Data analysis | pandas |
| Machine learning | scikit-learn |
| Development | Jupyter Notebook |
| Version control | Git, GitHub |

---

## Data

The dataset used for this project cannot be redistributed and is **not included** in this repository.

---

## Repository Structure

```text
telecom-customer-churn-prediction/
├── k_means.ipynb
├── random_forest.ipynb
└── README.md
```

---

## Methodology

1. Inspect and prepare the customer data for analysis.
2. Use k-means clustering to explore potential customer groups.
3. Evaluate clustering with a silhouette score.
4. Prepare the data for supervised churn prediction.
5. Train and validate a random forest classifier.
6. Evaluate the final classifier on a held-out test set using accuracy, precision, recall, F1, and ROC-AUC.

---

## Results

The k-means analysis produced a **silhouette score of 0.3576**. This suggests some grouping in the selected feature space, though the clusters were not strongly separated.

On the final test set, the random forest classifier achieved:

| Metric | Final test result |
|---|---:|
| Accuracy | 0.8807 |
| Precision | 0.8184 |
| Recall | 0.7295 |
| F1 score | 0.7714 |
| ROC-AUC | 0.9362 |

The classification results indicate that the model distinguished churners from non-churners well on this test set. Its recall also shows that it missed some customers who churned, an important consideration if the model were used to prioritize retention outreach.

---

## Key Features

- Separate notebooks for customer segmentation and churn prediction
- K-means clustering with silhouette-score evaluation
- Random forest churn classification
- Final test-set evaluation using multiple metrics
- Discussion of how the results could inform retention decisions

---

## Lessons Learned

This project strengthened my understanding of:

- The different questions answered by clustering and classification
- Preparing customer data for machine learning
- Evaluating clusters without overstating their separation
- Comparing classification metrics in the context of a business decision
- Communicating what a model's results do and do not establish

---

## Future Improvements

- Examine which customer characteristics most influence churn predictions
- Compare the random forest with a simpler baseline model
- Explore thresholds based on the cost and capacity of retention outreach
- Test whether the results hold on data from a later period
- Revisit clustering features and methods to assess whether more useful segments emerge

---

## About Me

I hold an M.S. in Data Analytics with an emphasis in Data Science from Western Governors University. My interests include data science, business analytics, and translating analytical findings into practical recommendations.
