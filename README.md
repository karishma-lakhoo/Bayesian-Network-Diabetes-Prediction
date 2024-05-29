# Bayesian-Network-Diabetes-Prediction
# Early Classification of Diabetes Diagnosis Using Bayesian Networks

This project aims to develop an early classification system for diabetes diagnosis using Bayesian Networks, a class of Probabilistic Graphical Models (PGMs). It compares three different Bayesian Network models: a custom model based on domain knowledge and empirical findings, an unconstrained Hill Climb model learned from data, and a constrained Hill Climb model incorporating domain knowledge through blacklisted edges.

## Dataset

The dataset used in this project is the "Early Classification of Diabetes" dataset obtained from Kaggle. It contains observations with 17 features collected from patients in the Sylhet Diabetes Hospital in Bangladesh.

## Approach

1. **Data Handling and Preprocessing:** The dataset was preprocessed, and exploratory data analysis was conducted to identify potential relationships between variables.
2. **Model Selection and Application:** Three Bayesian Network models were developed:
   - Custom model based on domain knowledge and empirical findings
   - Unconstrained Hill Climb model learned from data
   - Constrained Hill Climb model incorporating domain knowledge through blacklisted edges
3. **Structure Learning and Parameter Estimation:** The Hill Climb Search algorithm with the BIC scoring function was used for structure learning. The Bayesian Dirichlet equivalent uniform (BDeu) prior was used for parameter estimation.
4. **Inference and Results Analysis:** Exact inference using the Variable Elimination method was performed to compute posterior probabilities and analyze the captured relationships between features and the target variable.
5. **Hyperparameter Tuning:** The maximum indegree parameter was tuned to optimize model performance.
6. **Evaluation:** The models were evaluated using accuracy, precision, recall, and F1 score metrics on test and validation datasets.


## Results

The evaluation results highlight the strengths and limitations of various approaches to learning Bayesian Networks for diabetes prediction. The unconstrained Hill Climb model achieved the best performance after hyperparameter tuning, with high accuracy, precision, recall, and F1 score on the test dataset.


