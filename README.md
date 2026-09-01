# iris_ KNN
iris classification using logistic regression and Sk learn  
This project focuses on the classification of Iris flower species using machine learning techniques in Python. The Iris dataset was used to develop and evaluate a classification model based on flower measurements such as sepal length, sepal width, petal length, and petal width.

The dataset was loaded and processed using Pandas, NumPy, and Scikit-learn. The feature variables (X) represent the four Iris flower measurements, while the target variable (y) represents the corresponding Iris species.
Data Preparation
The Iris dataset was converted into a Pandas Data Frame. The feature columns were assigned using the Iris feature names, and the target column was named Species. The first five rows of the dataset were displayed to verify the data and its structure.
The dataset was then divided into training and testing datasets using an 80:20 ratio. Thus, 80% of the data was used for training the model and 20% was used for testing its performance. A random state value of 42 was used to ensure reproducibility.
Model Development
A K- Nearest Neighbours (KNN) Classifier from Scikit-learn was used for Iris species classification. The value of K was set to 5, meaning that the model considers the five nearest data points when determining the class of a new observation.
The model was trained using the training features (X_ train) and training target values (y_ train). After training, predictions were generated for the test dataset using X_ test.
Model Evaluation
The performance of the trained KNN classification model was evaluated using several metrics:
Accuracy Score: Measures the overall percentage of correctly classified Iris samples.
Confusion Matrix: Shows the number of correctly and incorrectly classified samples for each Iris species.
Classification Report: Provides detailed evaluation metrics, including precision, recall, F1-score, and support for each class.
These evaluation methods help determine how effectively the model distinguishes between the different Iris species.
Prediction of a New Flower
To test the model on an unseen observation, a new Iris flower was provided with the measurements:
[5.1, 3.5, 1.4, 0.2]
The trained KNN model was used to predict the species of this new flower. The predicted numerical target value was then mapped to the corresponding Iris species name using the target names from the dataset.
For this particular measurement, the predicted target is 0, which corresponds to Iris setosa.
