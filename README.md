# Near-Earth-Object-Hazard-Classification
Near-Earth Object Hazard Classification

### Overview
This project aims to classify Near-Earth Objects (NEOs) as potentially hazardous or not using machine learning techniques. The dataset contains information about various NEOs, including their size, velocity, and distance from Earth. The classification model predicts whether an NEO is hazardous based on these features.

### Project Structure
Data Preprocessing: Cleaning the dataset by removing missing values, encoding categorical variables , and scaling the numerical features.
Model Training: A Logistic Regression model is trained to classify whether an NEO is hazardous.
Model Evaluation: The model's performance is evaluated using key classification metrics: Precision, Recall, F1-Score, and AUC-ROC.

### Data Preprocessing
The dataset was cleaned by:

  Fill rows with missing values.
  Converting categorical variables, such as orbiting_body, using one-hot encoding.
  Dropping irrelevant features such as neo_id and name, which are non-numeric and not useful for classification.
  Scaling numerical features using StandardScaler to ensure they are on the same scale for training.
  Model Training
  The machine learning model used is Logistic Regression, a simple yet effective algorithm for binary classification. The target variable is is_hazardous,     
  indicating whether an NEO is potentially hazardous.

### Evaluation Metrics
The model is evaluated using the following metrics:

  Precision: Measures the proportion of correctly predicted hazardous objects out of all objects predicted as hazardous.
  Recall: Measures the proportion of actual hazardous objects that were correctly identified by the model.
  F1-Score: A balanced metric that combines Precision and Recall. It is useful when both false positives and false negatives are important.
  AUC-ROC: Evaluates how well the model distinguishes between hazardous and non-hazardous objects, plotting the true positive rate against the false positive rate.

### AUC-ROC Curve
The AUC-ROC curve provides a graphical representation of the model's performance across various thresholds. A higher AUC score indicates that the model is better at distinguishing between the two classes (hazardous and non-hazardous).
