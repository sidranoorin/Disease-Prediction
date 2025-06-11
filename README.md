# Disease-Prediction
Disease Prediction Using Machine Learning
This project demonstrates an end-to-end implementation of a disease prediction system using machine learning. It aims to assist healthcare professionals by providing accurate and early diagnoses based on patient symptoms.

📌 Overview
The system takes a list of symptoms as input and predicts the most likely disease using a combination of machine learning models. It addresses data imbalance, evaluates model performance with cross-validation, and uses ensemble methods to improve prediction accuracy.

⚙️ Features
Data preprocessing and label encoding
Class distribution visualization
Handling class imbalance using RandomOverSampler
Model evaluation using Stratified K-Fold Cross-Validation
Training and comparison of multiple ML models
Ensemble prediction using majority voting (mode)
User-defined prediction function for real-time use

🧰 Libraries Used
pandas
numpy
scipy
matplotlib
seaborn
scikit-learn (sklearn)

📊 Data Processing
Load Dataset
The dataset is loaded and disease labels are encoded into numerical format for model training.

Class Distribution Visualization
A plot of class distribution is generated to check for class imbalance.

Balancing the Dataset
The RandomOverSampler from imblearn is used to duplicate minority class samples, ensuring each disease class has an equal number of samples.

🤖 Model Training & Evaluation
Stratified K-Fold Cross-Validation
To maintain representative class proportions, a 2-split stratified K-fold approach is used due to smaller class sizes.

Model Selection
Three machine learning models are trained and evaluated.

Confusion Matrix
Used to visualize the performance of each model on the test set.

🔁 Ensemble Method
To build a more robust prediction system, we combine predictions from all three models using majority voting (mode). This reduces the effect of individual model errors.

🧪 Disease Prediction Function
A custom function takes user-provided symptoms, encodes them into numerical format, and predicts the disease using the ensemble model.

