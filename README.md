# HW-21-Challenge
Module 21 Challenge


# Alphabet Soup Nonprofit Foundation Funding Model

## Introduction

This repository contains a project focused on selecting applicants for funding by the nonprofit foundation Alphabet Soup. The project involves working with a large dataset to create a predictive model for successful funding outcomes. The primary target variable in this project is "Is_successful," and we have considered two key feature variables for our modeling: "CLASSIFICATION" and "APPLICATION_TYPE."

## Initial Model

In our initial modeling phase, we made several decisions:

- We excluded the "NAME" and "EIN" variables due to their string values, which were challenging to incorporate into the initial model.
- We selected the activation functions "ReLU" for its speed and "Sigmoid" for its predictive performance.
- The number of neurons and hidden layers was chosen as a starting point, with a mix of even and odd numbers to evaluate their impact on model accuracy.

## Model Iterations

After running the first neural network model, I aimed to improve the accuracy metric through feature adjustments. We applied binning to the "NAME" feature and scaled the data. I re-implemented the baseline algorithms and created three additional neural network models:

### Model 2

- Utilized four neurons in the hidden layers.
- Set the epoch value to 150.
- Maintained "ReLU" activation for hidden layers and "Sigmoid" for prediction.

### Model 3 (Best Performing)

- Utilized three hidden layers.
- The first layer contained 10 neurons, the second layer had 6 neurons, and the third layer had 3 neurons.
- Achieved the highest accuracy of 73% among the models.
- Precision and recall slightly outperformed models 2 and 4.

### Model 4

- Used four hidden layers with varying neuron counts (8, 6, 4, and 2).
- Achieved a similar accuracy score of 72% as models 2 and 3.

## Future Improvements

The success of Model 3 suggests that further feature engineering, experimentation with the number of neurons in each layer, and exploring odd numbers of hidden layers may lead to even better results. While neural network models have shown promise, it's worth considering a linear regression model for its simplicity and interpretability, especially for stakeholders who may require a more straightforward understanding of the model.

## Conclusion

In summary, this project aims to identify the best applicants for funding by Alphabet Soup using predictive modeling techniques. I have explored various neural network models and achieved promising results, with room for further optimization. The choice between complexity and interpretability will be carefully considered as I continue to refine future models.

