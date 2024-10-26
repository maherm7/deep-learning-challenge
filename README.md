# deep-learning-challenge

Data Preprocessing

Target Variable(s):
IS_SUCCESSFUL: This column indicates if previous funding was used effectively, which serves as the target variable for the binary classification.



Feature Variable(s):

APPLICATION_TYPE: Type of application submitted.
AFFILIATION: Sector of industry with which the organization is affiliated.
CLASSIFICATION: Government classification for the organization.
USE_CASE: Purpose or intended use of the requested funding.
ORGANIZATION: Type of organization applying for funding.
STATUS: Active status of the organization.
INCOME_AMT: Classification of the organization’s income level.
SPECIAL_CONSIDERATIONS: Notes any special considerations for the application.
ASK_AMT: The amount of funding requested by the applicant.



Variables Removed:

EIN and NAME: These columns are unique identifiers that do not contribute to the prediction of success, so they were removed to avoid unnecessary complexity.
Compiling, Training, and Evaluating the Model



Model Architecture:

Neurons: The model uses 30 neurons in the hidden layers, determined through tuning to balance model complexity and performance.
Layers: A multi-layer architecture with an input layer, hidden layer, and an output layer. This layered structure effectively captures patterns in the data without leading to overfitting.



Activation Functions:

ReLU (Rectified Linear Unit) for hidden layers: This choice allows for non-linear transformations, improving the model's ability to capture complex patterns.
Sigmoid for the output layer: Ideal for binary classification as it provides a probability score for each prediction.



Model Performance:

Target Achievement: The goal was to achieve an accuracy rate of at least 75-80%.



Performance Improvement Steps:

Normalization: Standardizing feature scales allowed for faster and more stable training.
Hyperparameter Tuning: Adjusted the number of neurons, batch size, and learning rate.
Epochs Adjustment: Decreased based on convergence trends, aiming to optimize training time without overfitting.



Model Evaluation Results
Accuracy and Loss: Key performance metrics are displayed here.



Summary
The deep learning model produced significant insights into the factors influencing funding success at Alphabet Soup. While the model meets initial performance benchmarks, there may be alternative approaches that could further enhance its predictive accuracy. For example, using a Random Forest Classifier may provide a more interpretable model that also excels in handling categorical data, especially with a large number of features. Additionally, ensemble techniques could yield robust predictions and offer insights into the importance of specific features.

