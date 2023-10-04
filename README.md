# Resume_Prediction
A machine learning pipeline for text classification using resumes as an example dataset. The code includes data preprocessing, model training, prediction, and evaluation components. 

# Key Components 

Data Loading: The code begins by loading the resume data from a CSV file using pandas. The dataset contains two columns: "Resume" (text data) and "Personality_Labels" (target labels).

Text Preprocessing: To prepare the textual data for modeling, it uses the TF-IDF (Term Frequency-Inverse Document Frequency) vectorization technique. The TF-IDF vectorizer converts the text into numerical features suitable for machine learning.

Data Splitting: The dataset is split into training and testing sets using the train_test_split function from scikit-learn. This ensures that there's a portion of data reserved for evaluating the model's performance.

Model Selection and Training: In this code, a Logistic Regression model is chosen as an example. The selected model is then trained on the training data using the fit method.

Model Prediction: After training, the model is used to make predictions on the testing data using the prediction method. The predicted labels are stored in the y_pred variable.

Evaluation: The code proceeds to evaluate the model's performance using two types of visualizations:

Confusion Matrix Heatmap: A confusion matrix is generated to visualize the number of true positives, true negatives, false positives, and false negatives. This helps in assessing how well the model is performing for each class.

Classification Report: A classification report is created using the classification_report function. It provides detailed metrics such as precision, recall, F1-score, and support for each class. This report gives a more comprehensive overview of the model's performance.

Visualization: The confusion matrix heatmap is displayed using Matplotlib and Seaborn. The heatmap provides a visual representation of the model's classification results.

Printed Classification Report: The classification report is printed to the console, providing detailed metrics for each class, including precision (accuracy of positive predictions), recall (sensitivity), F1-score (harmonic mean of precision and recall), and support (number of occurrences of each class).
