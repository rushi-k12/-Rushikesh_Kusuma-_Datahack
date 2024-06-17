
# Vaccine Prediction Project
This project aims to predict the likelihood of individuals receiving the XYZ flu vaccine and the seasonal flu vaccine. The predictions are based on a variety of features such as demographic information, health behaviors, and opinions on vaccine effectiveness.
## Project Description
The goal of this project is to predict the probabilities of respondents receiving two types of flu vaccines: XYZ flu vaccine and seasonal flu vaccine. The predictions are made using a variety of features such as demographic information, health behaviors, and opinions on vaccine effectiveness. The performance of the model is evaluated using the area under the receiver operating characteristic curve (ROC AUC) for each of the two target variables.

## Project Structure
training_set_features.csv: Training data features
training_set_labels.csv: Training data labels
test_set_features.csv: Test data features
submission_format.csv: Submission format with respondent IDs
## Files
vaccine_prediction.ipynb: Jupyter Notebook containing data preprocessing, model training, and prediction steps.
submission.csv: Final submission file with predicted probabilities for each respondent.
README.md: This file.
## Steps to Reproduce
### 1. Environment Setup
Make sure you have the necessary Python libraries installed. You can use the following command to install the required libraries:
### 2. Data Preprocessing
Loaded the datasets using Pandas.
Handle missing values:
For numerical columns, filled missing values with the median.
For categorical columns, filled missing values with the mode.
One-hot encode categorical variables.
### 3. Model Training
Used a RandomForestClassifier wrapped in MultiOutputClassifier to handle the multilabel classification.
Trained the model using the training features and labels.
### 4. Prediction
Made predictions on the test set.
Extracted probabilities for both xyz_vaccine and seasonal_vaccine.
### 5. Submission File
Created  the submission file in the required format.

### Final Notes
Make sure to validate the final submission file before uploading it to the competition platform. Ensure that the columns respondent_id, xyz_vaccine, and seasonal_vaccine are correctly populated.
