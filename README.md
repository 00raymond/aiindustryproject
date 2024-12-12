# Model Comparison with Heart Disease Dataset
Dataset sourced from UCI ML repository.
## Data Pre-processing
- _Filling empty data entries_:
After identifying null values in our data, we fill using K-Nearest-Neighbors algorithm since we have many features which contribute to the classification of the disease.
- _Anomaly Detection_:
Isolation Forest is used to identify anomalies since we have high-dimensional data-- we are dealing a large amount of features.

## Model Generation
- _Metrics_: The comparison performed on the models is made using the following metrics: **f1 score, recall, precision, and roc auc**
- _Models_: We utilize classification models XGBoost, Random Forest, and Support Vector.
- _Parameters_: To find optimal hyperparameters during runtime we use GridSearchCV.

## Further evaluation (SHAP)
- SHAP visualizes the weight of each feature and how much each feature contributes towards the classification.
