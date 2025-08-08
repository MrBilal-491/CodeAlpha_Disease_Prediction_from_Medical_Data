# CodeAlpha_Disease_Prediction_from_Medical_Data
The main goal of this project is to develop a disease prediction model using structured patient data such as test results, demographic information, and medical features. By leveraging machine learning, we aim to predict the presence or absence of a disease, thereby assisting in early diagnosis and better treatment planning.
Dataset Description
For this study, we used the Breast Cancer Wisconsin Diagnostic Dataset, which is a well-known and publicly available dataset in the sklearn.datasets library. It contains 569 patient records with 30 real-valued features derived from digital images of fine needle aspirates (FNA) of breast masses.
🔑 Key Features:
•	Radius (mean of distances from center to points on the perimeter)
•	Texture (standard deviation of gray-scale values)
•	Perimeter, Area, Smoothness, Compactness, Concavity, Symmetry
•	…and other domain-specific features.
🎯 Target Labels:
•	0: Malignant (cancerous)
•	1: Benign (non-cancerous)
________________________________________
Approach
To solve this classification problem, the pipeline follows these steps:
1. Data Preprocessing
•	Train-Test Split: The dataset is divided into training and testing sets (80/20).
•	Feature Scaling: Standardization is applied to normalize features for algorithms that are sensitive to scale (e.g., SVM, Logistic Regression).
2. Model Training
We apply four supervised machine learning classification algorithms:
________________________________________
🔍 Algorithms Used
1. Logistic Regression
•	A statistical model used for binary classification.
•	Models the probability that a given input point belongs to a particular class.
•	Output is interpreted using the sigmoid function, which maps values between 0 and 1.
2. Support Vector Machine (SVM)
•	SVM creates a hyperplane that best separates the classes in the feature space.
•	It is effective in high-dimensional spaces and works well when the margin between classes is clear.
•	We used the variant that supports probability estimation.
3. Random Forest
•	An ensemble method based on Decision Trees.
•	It creates a large number of trees during training and outputs the mode of the classes.
•	Excellent for handling overfitting and non-linear relationships.
4. XGBoost (Extreme Gradient Boosting)
•	A highly efficient and accurate implementation of gradient boosting.
•	It builds trees sequentially, where each new tree corrects the errors made by previous ones.
•	Known for its speed and accuracy, especially in structured data.
