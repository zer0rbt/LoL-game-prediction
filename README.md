### Understanding the League of Legends Match Outcome Prediction Project

#### Introduction to League of Legends
League of Legends (LoL) is a highly popular multiplayer online battle arena (MOBA) game developed by Riot Games. In LoL, two teams of five players each compete to destroy the opposing team's Nexus, which is the core building located in their base. The game combines elements of strategy, teamwork, and quick decision-making. Each player controls a character known as a "champion," each with unique abilities and roles.

#### Objective of the Project
The primary goal of this project is to predict the outcome of a match (whether the blue team wins or loses) using various machine learning models. By analyzing in-game data, I aim to understand what factors contribute most to winning and losing, and how these factors differ across player rankings.

#### Data Description
The dataset used in this project includes detailed statistics from League of Legends matches. Each match is represented by various features (attributes) that capture different aspects of the game, such as:
- **Team Gold**: Total gold earned by a team, which is crucial for purchasing items that enhance champion abilities.
- **Kills and Deaths**: Number of enemy champions killed and the number of times champions died.
- **Experience Points (XP)**: Earned to level up champions and unlock stronger abilities.
- **Towers Destroyed**: Indicates how many defensive structures of the enemy team have been destroyed.

The target variable I aim to predict is `blueWins`, a binary variable indicating whether the blue team won the match.

#### Machine Learning Models Used
To predict the match outcomes, I used the following classification algorithms:

1. **Decision Tree Classifier**: This algorithm splits the data into subsets based on feature values, creating a tree-like structure where each leaf node represents a class label (win or lose).

2. **Random Forest Classifier**: An ensemble method that builds multiple decision trees and combines their outputs. It provides higher accuracy and stability by averaging the results from many trees.

3. **Logistic Regression**: A statistical model that estimates the probability of a binary outcome (win or lose) based on input features. It is effective for understanding the influence of each feature on the prediction.

4. **Naive Bayes Classifier**: Based on Bayes' theorem, it assumes that features are independent and calculates the probability of each class. Despite its simplicity, it performs well on large datasets.

#### Data Preprocessing
Before training the models, I preprocess the data to ensure it is clean and suitable for analysis:
- **Deleting unique values**: I deleted unique values (such as match Id)
- **Feature and Target Separation**: We separate the dataset into features (input variables) and the target variable (`blueWins`).

#### Separate Analysis for Different Rankings
To account for different gameplay dynamics and strategies at various skill levels, I conducted separate analyses for two player rankings:
- **Diamond**: A high-ranking level where players have a deep understanding of game mechanics and strategies.
- **Grandmaster**: One of the top tiers in LoL, where players exhibit exceptional skill and coordination.


#### Conclusion
By leveraging multiple machine learning algorithms and conducting separate analyses for different player rankings, I aim to provide a comprehensive understanding of match outcomes in League of Legends. This project not only enhances prediction accuracy but also offers valuable insights into the factors influencing game results, helping players and analysts better understand the dynamics at different skill levels.

This project provides a foundation for further exploration and analysis of in-game data, potentially leading to strategies that can improve player performance and team success in League of Legends.