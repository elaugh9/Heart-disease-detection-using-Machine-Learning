# Heart-disease-detection-using-Machine-Learning
Many predictive models are being used in different medical domains. With the variety of options, the most used models in diagnostic and prognostic tasks are logistic regression (LR) and artificial neural networks (ANN). We will use UCL Cleveland Heart Disease dataset that consists of 303 examples and 14 features. The dataset is split into a training set, validation set, and testing set. The project workflow consists of two steps, training the models, and testing them. In this report, we show the results of training artificial neural networks, and logistic regression with and without normalization. Then we proceeded by comparing the results and explaining why training artificial neural networks outperform logistic regression
# Introduction
  Many predictive models are being used in different medical domains. With the variety of options, the most used models in diagnostic and prognostic tasks are logistic regression (LR) and artificial neural networks (ANN) [1]. We will use UCL Cleveland Heart Disease dataset that consists of 303 examples and 14 features. The dataset is split into a training set, validation set, and testing set. The project workflow consists of two steps, training the models, and testing them. In this report, we show the results of training artificial neural networks, and logistic regression with and without normalization. Then we proceeded by comparing the results and explaining why training artificial neural networks outperform logistic regression.
  
# Functions
In order to accomplish the task, we implemented 7 functions:

1. normalizeFeatures(x) : x
2. sigmoid(z): g
3. computeLRCost(x, y, theta, lambda): [cost, grad]
4. learnLRTheta(x, y, lambda): theta
5. trainLRModel(x, y, lambda_values): [theta, lambda]
6. predictClass(x, theta, threshold): y
7. testPerformance(y, y_predicted): [acc, recall, precision, fScore]

# Experiment
  After completing our implementation, we applied the following experiments and reported their results below:
  
# Experiment 1: logistic regression without feature normalization
  Due to some mathematical complications, we had to use a very small learning rate (0.0003), otherwise, the log() = infinity. Training (blue) and validation (yellow) errors Vs. lambda values curve is shown in the following figure:
