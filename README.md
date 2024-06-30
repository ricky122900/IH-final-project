# IH-final-project
## Title: Telco Customer Churn Prediction

## Project Overview
This project aims to predict customer churn for Telco, a telecommunications company in California. By accurately predicting churn, the company can implement targeted retention strategies to reduce customer loss and improve overall business performance.

## Dataset
The dataset was sourced from Kaggle and originally consisted of 52 columns and 5634 rows. It included a training set, test set, and validation set.

### Data Description
- **Columns:** 52
- **Rows:** 5634
- **Key Features:** Age, Location, Gender, Services Subscribed to, Churn Score, Customer Status, etc.
- **Target Variable:** Churn Value (1 for churned, 0 for not churned)

### Data Cleaning
- Only 2 columns had null values, which were insignificant and filled with 'Unknown'.
- Columns were lowercased and spaces were replaced by underscores.
- Basic data cleaning was done.

## Exploratory Data Analysis (EDA)
- **Age Distribution:** Mean age was 46, range 61, mode 42.
- **Churn Score:** Mean churn score was 58.
- **Top Cities:** Los Angeles and San Diego had the most customers.
- **Target Variable Distribution:** Data was imbalanced with 4139 not churned and 1495 churned.

## Data Preprocessing
- **Handling Imbalanced Data:** Applied SMOTE to handle class imbalance.
- **Label Encoding:** Converted categorical columns to numeric using label encoding.
- **Feature Selection:** Reduced the number of features from 51 to 14 based on correlation analysis to improve model performance.

## Model Building
Several models were tested including:
- K-Nearest Neighbors (KNN)
- Decision Tree
- Bagging and Pasting
- Random Forest
- Gradient Boosting
- ADA Boost
- SMOTE

### Best Model
- **Model:** Bagging and Pasting
- **Hyperparameter Tuning:** Conducted and slightly improved the model performance.

## Model Evaluation
- **Training Set Performance:** Evaluated using accuracy, precision, recall, and F1 score.
- **Validation Set Performance:** The model correctly predicted 1384 out of 1409 records with only 25 incorrect predictions.
- **Confusion Matrix:** 16 false negatives and 9 false positives.

## Key Findings
- **Age and Churn Likelihood:** Older customers are more likely to churn.
- **Marital Status and Churn:** Customers who are married or live with someone are less likely to churn.
- **Geographic Insights:** San Diego faces significant competition, prompting a decision to either drop the branch or make major improvements.
- **Data Quality and Model Performance:** High-quality churn behavior data is crucial for building an effective predictive model.

## Tableau Visualizations
- Created an interactive dashboard in Tableau to visualize churn rates by city, by gender, by maritial status and by age. Also, each categories distribution can also be visualized. Visuals were published in Tableau Public and here is the link: https://public.tableau.com/app/profile/ricardo.torres5908/viz/customer-churn-visualizations/Dashboard1?publish=yes 

## Conclusion
- **Business Implications:** Implement targeted retention strategies for older customers and promote family-oriented packages. Conduct a cost-benefit analysis for the San Diego branch.
- **Future Work:** Enhance data collection methods, regularly update and retrain the model, and explore additional features affecting churn.

## Link for the Trello Board used for project management: https://trello.com/b/uC2vsrBE/final-project-board
## Link for Canva Presentation: https://www.canva.com/design/DAGJZaSESTk/nD5SQVjC0-sJgczpRZtT8Q/edit?utm_content=DAGJZaSESTk&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton 