Parkinson’s Disease Detection
Overview
The Parkinson’s Disease Detection project is a machine learning-based application designed to enable early detection of Parkinson’s disease (PD) using vocal biomarkers. By analyzing voice features such as pitch, jitter, and shimmer, the system classifies whether a patient exhibits signs of PD, achieving a high accuracy of 97.83%. This project demonstrates the potential of non-invasive, data-driven diagnostics to assist clinicians in identifying PD early, improving patient outcomes.
Objectives
•  Develop a machine learning model to accurately detect Parkinson’s disease from vocal data.
•  Explore multiple machine learning algorithms to identify the most effective approach for PD classification.
•  Create a scalable and interpretable system to support healthcare applications.
Methodology
•  Dataset: Utilized a vocal biomarker dataset containing features like fundamental frequency, jitter, shimmer, and other speech metrics associated with Parkinson’s disease symptoms.
•  Preprocessing: Cleaned the dataset by handling missing values and standardizing features to ensure consistent scales for model training.
•  Modeling: Trained and evaluated multiple machine learning algorithms, including:
	•  AdaBoost
	•  CatBoost
	•  K-Nearest Neighbors (KNN)
	•  Linear Discriminant Analysis (LDA)
	•  Logistic Regression
•  Feature Engineering: Applied Principal Component Analysis (PCA) with various kernels to capture nonlinear patterns in the vocal data.
•  Evaluation: Used accuracy as the primary metric, with a 70-30 train-test split to assess model performance on unseen data.
•  Optimization: Experimented with different train-test splits and hyperparameters to maximize model accuracy and generalization.
Technologies Used
•  Programming Language: Python
•  Libraries:
	•  scikit-learn (for machine learning models and PCA)
	•  Pandas (for data preprocessing)
	•  NumPy (for numerical operations)
•  Dataset: Vocal biomarker dataset for Parkinson’s disease (sourced from [add source if known, e.g., UCI Machine Learning Repository, or leave as is])
Key Features
•  Non-Invasive Diagnosis: Uses vocal features for a non-invasive approach to PD detection.
•  High Accuracy: Achieved 97.83% accuracy using the AdaBoost Classifier, outperforming other models.
•  Robust Evaluation: Tested models with various train-test splits and PCA kernels to ensure reliable performance.
•  Scalable Framework: Designed to be adaptable for other medical diagnostic tasks with similar data.
Usage
•  Input: The script expects a CSV file with vocal features (e.g., jitter, shimmer, fundamental frequency).
•  Output: The model outputs predictions (PD or non-PD) and prints the accuracy, along with a classification report showing precision, recall, and F1-score.
•  Customization: Modify the parkinsons_detection.py script to adjust train-test splits, try different models, or tune hyperparameters.
Results
•  Model Performance: The AdaBoost Classifier achieved the highest accuracy of 97.83% on a 70-30 train-test split, demonstrating strong predictive power.
•  Comparative Analysis: Outperformed other models like CatBoost, KNN, LDA, and Logistic Regression in accuracy.
•  Impact: The high accuracy and use of vocal biomarkers highlight the potential for non-invasive, scalable PD diagnostics, supporting early intervention in clinical settings.
Challenges and Solutions
•  Challenge: Handling imbalanced or noisy vocal data.
	•  Solution: Applied data cleaning and standardization to ensure consistent feature scales.
•  Challenge: Selecting the best model for PD detection.
	•  Solution: Compared multiple algorithms, with AdaBoost proving most effective due to its ability to combine weak learners for robust predictions.
Future Enhancements
•  Integrate additional data modalities (e.g., movement or handwriting data) for multi-modal PD detection.
•  Implement real-time audio input for live vocal analysis.
•  Explore deep learning models like LSTMs to capture temporal patterns in voice data.
•  Deploy the model as a web or mobile application for clinical use.
Contributing
Contributions are welcome! Please fork the repository, create a new branch, and submit a pull request with your improvements. For major changes, open an issue to discuss your ideas.
License
This project is licensed under the MIT License. See the LICENSE file for details.
