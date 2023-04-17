# Rainfall Prediction with Genetic Algorithm-Based Feature Selection

## Author

**Namya Vyas**

## Overview

This project implements a rainfall forecasting system that uses Genetic Algorithms (GA) for feature selection in a binary classification model. The system predicts whether it will rain tomorrow (`Yes`/`No`) using weather data from Australia.

By applying GA, the feature set is optimized to improve the classifier’s performance compared to traditional models, taking advantage of the randomness and evolutionary search capability of GA.

## Aim

* Perform feature selection using Genetic Algorithm in a binary rainfall prediction model.
* Optimize classifier performance and robustness by selecting an ideal subset of features.
* Demonstrate applicability in domains such as agriculture, tourism, and urban planning.

## Motivation

* Unlike deterministic statistical or regression models, GAs use randomness and historical information to discover better solutions.
* Helps avoid overfitting and improves generalization.
* Enables exploration of feature spaces not easily reached by typical algorithms.

## Methodology

### Genetic Algorithm Workflow

1. Initialize a population of candidate solutions (feature subsets).
2. Evaluate fitness of each individual by training and testing classifiers.
3. Select the best-performing individuals as parents.
4. Apply crossover and mutation to produce the next generation.
5. Repeat until stopping criteria are met (number of generations or convergence).

## Dataset

* Source: Bureau of Meteorology, Australia ([link](http://www.bom.gov.au/climate/data))
* Preprocessed version available via Kaggle
* Contains over 10 years of daily weather observations
* Target variable: `RainTomorrow` indicating if rainfall ≥ 1mm was recorded the next day

## Results

* GA-based feature selection improved classifier performance by approximately 1–2% when using KNN and Radial SVM classifiers.
* Other classifiers (Linear SVM, Logistic Regression, Random Forest, AdaBoost, Decision Tree) showed overfitting with this dataset.

## Dependencies

* Python 3.x
* NumPy
* Pandas
* scikit-learn
* matplotlib or seaborn (optional, for visualizations)

## Future Work

* Evaluate performance on larger and different datasets for generalization.
* Extend the model to multi-class or probabilistic rainfall prediction.
* Integrate the model with live weather data feeds for real-time prediction.

## License and Attribution

* Dataset copyright: Commonwealth of Australia 2010, Bureau of Meteorology
* For educational and research purposes only