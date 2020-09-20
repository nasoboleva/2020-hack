# Team: Pumped Up Cheeks

## Description

Current repository contains Jupyter notebooks, which solve 
problems for `Tinkoff` hackaton. 

There are two main parts:
1. Improving proposed baseline.
2. The development of our model to predict `Tinkoff` product.

## Baseline improvement

Many approaches were tested during numerous experients,
but only the most successful solution is represented in 
`Improved_baseline.ipynb` notebook.

## Product prediction

Model for prediction of `Tinkoff` product has the following 
training procedure:
 - For each sample (which is equivalent to customer vector) random 
 `Tinkoff` product is selected.
 - In corresponding product vector selected product hides from the model
 by putting zero in corresponding position.
 - Target vector constructs as one-hot vector of chosen position.

This training procedure forces the model to guess missing product thus during inference stage learned model
predicts the product that suits current user the most.
