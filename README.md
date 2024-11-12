# Professional_portfolio-Machine-Learning
Predicting term deposit subscription likelihood using Random Forest.
Banking Industry: Predicting Term Deposit Subscription

Objective
This project aims to build a predictive model that estimates the likelihood of a customer subscribing to a term deposit based on historical marketing campaign data. The model assists banking institutions in identifying potential clients for term deposits, enabling more targeted and effective marketing campaigns.

Dataset
Source: Bank Marketing Dataset on Kaggle
Description: This dataset contains information on direct marketing campaigns conducted by a Portuguese banking institution. It includes 41,188 records with 20 features describing customer demographics, financial attributes, and campaign-specific features.

Features Used
Some of the key features used in this project include:
Age: Age of the client.
Job Type: Type of job the client has (e.g., admin, technician, blue-collar).
Marital Status: Marital status (e.g., married, single, divorced).
Education Level: Education level of the client.
Housing Loan: Whether the client has a housing loan.
Personal Loan: Whether the client has a personal loan.
Contact Type: Type of communication used for contact (cellular or telephone).
Previous Campaign Outcome: Outcome of previous campaigns (success, failure, nonexistent).
Days Since Last Contact: Number of days since the last contact.

Model and Methods
Machine Learning Algorithm: Random Forest
Class Balancing: Used SMOTE (Synthetic Minority Oversampling Technique) to address class imbalance in the dataset.
Feature Engineering: Grouped some categorical variables, created age categories, and converted certain numerical variables to binary.
Hyperparameter Tuning: Used Grid Search to optimize model parameters (e.g., n_estimators, max_depth).
Evaluation Metrics: Precision, Recall, F1 Score, and AUC-ROC to assess model performance.

Instructions to Run
Clone the Repository:

bash
Copy code
git clone https://github.com/subhasree1003/Professional_portfolio-Machine-Learning.git
cd Professional_portfolio-Machine-Learning

Install Required Libraries:
Ensure you have Python installed.

Open Jupyter Notebook:
bash
Copy code
jupyter notebook
Open bankdata.ipynb and run the cells to execute the code.

Additional Notes:
This project also requires the joblib library if you want to save or load the trained model. Install it via:
bash
Copy code
pip install joblib

Results
The Random Forest model achieved a balanced accuracy by adjusting class weights and using SMOTE for oversampling. Below are some of the key metrics:

Accuracy: 86.4%
Precision: 38.4% for the positive class
Recall: 33.4% for the positive class
AUC-ROC: 0.745
These results demonstrate the model’s effectiveness in identifying potential term deposit subscribers while maintaining a reasonable balance between precision and recall.

Future Improvements
Feature Engineering: Further refinement of feature groups and age segmentation.
Advanced Models: Testing other algorithms such as Gradient Boosting or XGBoost for improved prediction.
Dashboard: Integrate with Streamlit to create an interactive dashboard for real-time prediction and feature analysis.
