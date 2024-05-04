# Chapter 5. Feature Engineering

- feature engineering is the process of using domain knowledge to extract features from raw data via data mining techniques
- a large part of many ML engineering and data science jobs is to come up with new useful features
- having the right features tends to give them the biggest performance boost compared to clever algorithmic techniques such as hyperparameter tuning. State-of-the-art model architectures can still perform poorly if they don’t use a good set of features.

## Learned Features Versus Engineered Features

- feature learning is the process of automatically extracting features from raw data.
- deep learning models are able to learn features from raw data
- not all algorithms can learn features from raw data

## Common Feature Engineering Operations

- handling missing values
- deletion
- imputation
- feature scaling
- discretization
- Encoding Categorical Features
- feature crossing
- Discrete and Continuous Positional Embeddings

## Data Leakage

 Data leakage refers to the phenomenon when a form of the label “leaks” into the set of features used for making predictions, and this same information is not available during inference.

Common Causes for Data Leakage

- Splitting time-correlated data randomly instead of by time
- Scaling before splitting
- Filling in missing data with statistics from the test split
- Poor handling of data duplication before splitting
- Group leakage
- Leakage from data generation process

Detecting Data Leakage

## Engineering Good Features

- Feature Importance
- Feature Generalization
