
# Kubernetes Failure Prediction

Overview
This project predicts failures in Kubernetes clusters using a Random Forest classifier. The dataset consists of various performance metrics and categorical labels representing events in the cluster.

Repository Structure
/src → Code for data processing, training, and evaluation.
/models → Trained model and scaler.
/data → Dataset (`kubernetes_final_dataset.csv`).
/docs → Documentation.
/presentation → Presentation slides.

Requirements
Before running the project, ensure you have the following installed:
- Python 3.x
- Required libraries: `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `joblib`

How the Code Works
1. Load Data: Reads `kubernetes_final_dataset.csv` and fills missing values.
2. Encode Categorical Variables: Uses `LabelEncoder` for encoding categorical features.
3. Feature Selection: Chooses relevant features for training.
4. Train-Test Split: Splits the dataset into 80% training and 20% testing.
5. Feature Scaling: Uses `StandardScaler` for normalization.
6. Train Model: Fits a `RandomForestClassifier` with 100 trees.
7. Evaluate Model: Calculates accuracy and classification report.
8. Save Model: Saves the trained model and scaler for future use.
9. Visualize Decision Tree: Displays the first decision tree in the random forest.

Model Performance
The model achieves an accuracy of 32.4% due to the complexity of the dataset. Future improvements can be made by fine-tuning hyperparameters and feature engineering.

Submission Details
  Dataset Source:`data/kubernetes_final_dataset.csv`
  Trained Model:`models/https://drive.google.com/drive/folders/1jSND2keAULeS02ZfZA1v3btssAtsn529?usp=sharing`
  
