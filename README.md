## Description

This goal of this group project was to build a machine learning model that predicts the most accurately diabetes based on a [Kaggle dataset](https://www.kaggle.com/competitions/inf-8245-e-fall-2024) . It received a grade of 95% and it was done for the MILA Machine Learning class of Fall 2024 taught by Sarath Chandar.

A longer description of feature design, algorithms description, methodology, results and discussion can be found in the [Report](https://github.com/MurielleMardenli200/Diabetes_Prediction_Metamodel/blob/main/Report.pdf) of this repository.

## Model Description

The final meta model uses stacking methodology to combine a first base learner with a Bernoulli Naive Bayes (BNB) and a Logistic Regressor (LR). The BNB was chosen in order to make a univariate and multivariate analysis of the features.
 This extraction of information from the features combined with a logistic regressor improves feature representation for continuous and discrete variables.

The second base learner is an ANN. It was chosen because it models highly complex and non-linear relationships within the data.

Finally, a stacking ensemble method was chosen in order to combine the predictions of the previous models to obtain a better prediction as well as reduce both bias and variance.

## Results and Discussion

We examined the f1-score and the loss as a success indicator for the model. Through examination of F1-scores, we determined the ANN did most of the heavy lifting of the performance. we have concluded that this happens since the neural network extrapolates relations between all inputs whereas the Bernoulli-logistic approach limits itself to only a few combinations of binary and continuous features.

<img width="633" alt="Screenshot 2025-01-20 at 10 15 34 PM" src="https://github.com/user-attachments/assets/74cb8f41-49b4-4ab3-b9b4-0e564aa27c74" />
