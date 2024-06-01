### Predicting Match Outcomes in League of Legends

In this project, I aim to predict the outcome of matches in the popular online game, League of Legends. To achieve this, I have employed four different classification algorithms: Decision Tree, Random Forest, Logistic Regression, and Naive Bayes. Our analysis is focused on two distinct player rankings: Diamond and Grandmaster, which are considered to have different gameplay dynamics and strategies. Below, I provide an overview of each model and its role in our predictive analysis.
#### 1. Decision Tree Classifier
The Decision Tree classifier is a simple yet powerful algorithm that works by splitting the data into subsets based on the value of input features. It creates a tree-like model of decisions, where each node represents a feature, each branch represents a decision rule, and each leaf represents an outcome. The main advantages of using a Decision Tree include its interpretability and ease of visualization.

#### 2. Random Forest Classifier
The Random Forest classifier is an ensemble method that builds multiple decision trees and merges their results to obtain a more accurate and stable prediction. By averaging the predictions from various trees, the Random Forest reduces the risk of overfitting and improves generalization. This classifier is known for its high performance and robustness, especially in complex datasets with many features.

#### 3. Logistic Regression
Logistic Regression is a statistical method for analyzing datasets with one or more independent variables that determine an outcome. It predicts the probability of a binary outcome (win or lose in our case) based on a logistic function. Despite its simplicity, Logistic Regression is quite effective for binary classification tasks and provides clear insights into the influence of different features on the predicted outcome.

#### 4. Naive Bayes Classifier
The Naive Bayes classifier is based on Bayes' theorem and assumes independence between features. It calculates the probability of each class (win or lose) given the input features and chooses the class with the highest probability. Naive Bayes is particularly useful for large datasets and performs well even with the assumption of feature independence.

### Data Preprocessing
Before training these models, I preprocess the data to ensure it is clean and suitable for analysis. This includes:
- Splitting the dataset into features (X) and target (y), where the target variable is 'blueWins', indicating whether the blue team won the match.
- Deleting unique fields (like match id)

### Separate Analysis for Diamond and Grandmaster Rankings
We conducted separate analyses for Diamond and Grandmaster rankings to account for the different gameplay dynamics and strategies at these levels. This approach allows us to tailor our models to the specific characteristics and performance metrics of players within each ranking.

### Model Evaluation
To evaluate the performance of each classifier, I split the data into training and testing sets using a 80-20 split ratio. The models are trained on the training set and evaluated on the testing set. Key metrics for evaluation include accuracy.

### Conclusion
By utilizing multiple classification algorithms and separately analyzing the Diamond and Grandmaster rankings, I aim to leverage the unique strengths of each model and provide a comprehensive predictive analysis of match outcomes in League of Legends. This multi-model, multi-ranking approach not only enhances prediction accuracy but also offers insights into the factors influencing match outcomes, helping players and analysts better understand the game dynamics at different skill levels.