# Ensemble-Learning-Methods-Bagging-and-Stacking
The question-answer format repository for Ensemble Learning Methods Bagging and Stacking

## Pre-Requisite
Implement the following types of models for the tasks at hand. Make sure you
tune over necessary hyper-parameters and select the best-performing model.
1. Decision Trees (Can use sklearn)
2. Logistic and Linear Regressor for Classification and Regression respectively.
3. Multi-Layer Perceptron
   
Note that this list of models would henceforth be referred to as List 1 models

## Bagging
For both the classification and regression tasks do the following tasks:
1. Design a function that performs the bagging methodology of the ensemble
learning by taking as input the following parameters:

• Base Estimator Model  

– List 1 models  
• Number of Estimators  
– Variable according to the base estimator  
• Fraction/Number of Samples  
– 0.15, 0.25, 0.5, 0.75, 1.0  
• Bootstrap  
– True: Sampling with replacement is performed  
– False: Sampling without replacement is performed  
• Voting Mechanism:  
– Hard Voting: Every classifier has equal weight in the final output  
– Soft Voting: The final output is weighed by the confidence of the
base estimator models.  
3. For ease, assume the best hyper-parameters from sub-task 1 and train
ensemble models across all combinations of parameters specified above
and report the best-performing models.
4. Plot a heatmap for the accuracies obtained by each class of base estimator
models across Fraction of Samples and Number of Estimators (Keep other
parameters constant and to your choice)
5. Compare the performance of each model in List 1 models with the best-performing ensemble model of the same class with a single side-by-side
histogram
Note:
1. Voting Procedure: Every classifier specified above provides a confidence
probability that can be used for soft voting. For regression, divide the
dataset into train, val, and test splits and use the performance on the val
set as an insight for confidence.
## Stacking
Stacking is a general procedure where a learner is trained to combine the individual learners. Here, the individual learners are called the level-0 learners,
while the combiner is called the level-1 learner, or meta-learner.

1. Design a function that performs the bagging methodology of ensemble
learning by taking as input the following parameters:

• Level-0 estimators:  

– List 1 Models  

• Level-1 estimators:  

– Logistic and Linear Regressor for classification and regression
respectively  

– Decision Tree  

• Stacking Methodologies:  

– Stacking  

– Blending  

3. For ease, assume the best hyper-parameters from sub-task 1 and train
ensemble models across all combinations of parameters specified above
and report the best-performing models.
4. Compare the accuracies and the training time of the best-performing models of Bagging and Stacking ensembles of each Base Estimator Model class.


