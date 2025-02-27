1. Data Preprocessing:
Split dataset: Separate features (X) and the target variable (y).
Train-test split: Divide the dataset into training and testing subsets.
2. Train the Naive Bayes Classifier:
Initialize: Set up necessary data structures (likelihoods, class priors, predictor priors).
Calculate Class Priors: Compute the probability of each class in the target variable.
Calculate Likelihoods: For each feature, compute the likelihood of each feature value given each class.
Calculate Predictor Priors: Compute the probability of each feature value in the dataset (evidence).
3. Make Predictions:
For each test instance (query):
Initialize an empty dictionary to store posterior probabilities for each class.
For each class:
Calculate the posterior probability using Bayes' Theorem:
𝑃
(
𝑐
∣
𝑥
)
=
𝑃
(
𝑥
∣
𝑐
)
×
𝑃
(
𝑐
)
𝑃
(
𝑥
)
P(c∣x)= 
P(x)
P(x∣c)×P(c)
​
 
Select the class with the highest posterior probability.
4. Evaluate Accuracy:
Compare predicted labels with actual labels.
Compute accuracy by calculating the percentage of correct predictions.
Simple Step-by-Step Algorithm:
Preprocess Data:

Split dataset into X (features) and y (target).
Split data into training and test sets.
Train the Model:

Initialize data structures (likelihoods, class_priors, pred_priors).
For each class:
Calculate the prior probability of the class: P(c).
For each feature:
Calculate the likelihood of the feature values given the class: P(x|c).
Calculate the predictor priors: P(x) (probability of each feature value in the dataset).
Predict for a Query:

For each query:
For each class, calculate the posterior probability using Bayes' Theorem.
Choose the class with the highest posterior probability.
Evaluate Performance:

Compute the accuracy score for training and testing datasets.
This is a basic, high-level breakdown of the program’s workflow. The classifier is built by using conditional probability for each class given the features.
