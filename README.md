# neural-network-challenge-2

## Background
You are tasked with creating a neural network that HR can use to predict whether employees are likely to leave the company. Additionally, HR believes that some employees may be better suited to other departments, so you are also asked to predict the department that best fits each employee. These two columns should be predicted using a branched neural network.

## Goal

Predict for two different targets Department, a multi-class output, and Attrition, a binary output, with a single branched neural network.

## Summary

Mostly just followed the instructions to get the expected branches and paramters in the model. I used nunique to get the 10 features with the most unique values. These all happened to be numeric values, which made preprocessing straight-forward. I only did scaling. I did consider adding an 11th field, but it lowered the accuracy and increased the loss, so decided to leave it out.

## Improvements

Since I only used numeric fields, I'm sure there were some other fields that could have helped the outcome of the model if they were encoded. In particular, I could have tried adding 'JobRole'. This might improve the performance.

I wanted to utilize the balanced accuracy score to measure the model, but this required building a custom method. I was not able to get this to work and ran out of time, so I was forced to use the standard accuracy method.

Hyperparameter tuning was not done on this model and could improve it.