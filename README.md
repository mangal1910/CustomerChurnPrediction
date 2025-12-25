"# CustomerChurnPrediction" 
# Telco Customer Churn Prediction

## 📌 Project Overview
This project focuses on analyzing customer behavior in the telecommunications industry to predict customer churn. By leveraging machine learning, the project identifies key factors that contribute to customers leaving the service and builds a predictive model to classify customers as likely to "Churn" or "Stay."

## 📂 Repository Structure
* **`Telco_customer_Churn_Preduction.ipynb`**: The primary Jupyter Notebook containing the end-to-end workflow: data ingestion, cleaning, exploratory data analysis (EDA), and model building.
* **`Telco-Customer-Churn.csv`**: The dataset used for training and testing (input file).
* **`churn_model.pkl`**: The serialized machine learning model saved for future predictions.

## 📊 Dataset
The analysis uses the Telco Customer Churn dataset, which includes customer attributes such as:
* **Demographics:** Gender, Senior Citizen status, Partner, Dependents.
* **Services:** Phone Service, Multiple Lines, Internet Service, Online Security, Tech Support, Streaming TV/Movies.
* **Account Details:** Tenure, Contract, Paperless Billing, Payment Method, Monthly Charges, Total Charges.
* **Target:** `Churn` (Converted to binary: 1 for Yes, 0 for No).

## 🛠️ Key Features & Workflow
1.  **Data Preprocessing:**
    * Loading dataset using Pandas.
    * Handling missing values and data types.
    * Converting the categorical `Churn` column into a binary format.
2.  **Exploratory Data Analysis (EDA):**
    * Visualizing churn distribution.
    * Analyzing churn rates based on demographic factors (e.g., Gender, Partner status) using Seaborn count plots.
3.  **Model Training:**
    * Building a classification model to predict churn probability.
    * Saving the trained model using `joblib`.

## 💻 Requirements
To run this project, you will need Python and the following libraries:

```bash
pip install pandas seaborn matplotlib scikit-learn joblib