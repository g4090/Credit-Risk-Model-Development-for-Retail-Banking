# Credit-Risk-Model-Development-for-Retail-Banking
Project Objective:

Goal: To predict customer credit risk (whether a customer will default on a loan or not).

Target Variable: Default History (binary: 1 for default, 0 for non-default).

Steps Taken:

Data Preprocessing:

Loaded the dataset and handled missing values.

Applied One-Hot Encoding to categorical variables like Marital Status, Education Level, and Repayment Behavior.

Scaled numerical features like Age, Income, and Credit Balance using StandardScaler to ensure they are on the same scale.

Model Building:

Tried three models:

Logistic Regression (simple linear model).

Random Forest (ensemble model) with hyperparameter tuning.

XGBoost (gradient boosting model) to handle class imbalance and improve predictions.

Class Imbalance Handling:

Used SMOTE (Synthetic Minority Over-sampling Technique) to generate synthetic samples for the minority class (defaults).

Model Evaluation:

Evaluated models using metrics like accuracy, precision, recall, F1-score, and ROC-AUC.

Random Forest and XGBoost provided the best results but still struggled with predicting defaults due to class imbalance.

Challenges Faced:

Class Imbalance: The main challenge was that non-defaults were much more prevalent than defaults, making it difficult for models to predict defaults effectively.

Final Outcome:

The best-performing model after hyperparameter tuning was Random Forest, with an accuracy of 71% and better performance compared to Logistic Regression.

SMOTE improved the prediction of defaults but the model still had difficulty capturing defaults with high recall and precision.

Next Steps:

Further improvements can be made by exploring other ensemble models like LightGBM or trying deep learning models.

Hyperparameter tuning and resampling techniques like undersampling could be explored further.

Diagram to Visualize the Process
A flow diagram can help in visualizing the process and provide clarity when explaining your project to others.

Here’s a simple flowchart you can use:

plaintext
Copy
Edit
  +--------------------------------------------+
  |                Data Collection            |
  +--------------------------------------------+
                    |
                    v
  +--------------------------------------------+
  |             Data Preprocessing            |
  | - Handle missing values                  |
  | - One-Hot Encoding for categorical data   |
  | - Scale numerical features               |
  +--------------------------------------------+
                    |
                    v
  +--------------------------------------------+
  |           Model Building and Training     |
  | - Logistic Regression                     |
  | - Random Forest (with SMOTE)             |
  | - XGBoost                                |
  +--------------------------------------------+
                    |
                    v
  +--------------------------------------------+
  |           Model Evaluation and Tuning     |
  | - Accuracy, Precision, Recall, F1-Score   |
  | - Hyperparameter Tuning                   |
  +--------------------------------------------+
                    |
                    v
  +--------------------------------------------+
  |           Results & Insights              |
  | - Best Model: Random Forest               |
  | - Accuracy: 71%                           |
  | - Further work: Handle Class Imbalance    |
  +--------------------------------------------+
