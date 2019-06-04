# issue-detection

This project is based on the [Issue-Label-Bot](https://github.com/machine-learning-apps/Issue-Label-Bot) project with some adjustments.

# Adjustments:

### Simplified model training

The project only contains functions to retrieve and preprocess data and train the model. No other features (e.g. Github App) are included.

### Binary Classification Problem

Further projects need only to distinguish between issues with bug or non bug description. Therefore, all issues labeled as "questions" are put in the same class.

### Model uploaded

As the process of retrieving, preprocessing and training consumes a large amount of memory (and time), this project contains the current best model as HDF5 file.

# Further work

- Split data in three sets and compute evaluation output (precsision, recall, etc.)
- Experiment with more complex models to get better results (above 81% accuracy)
- Create pipeline to retrieve new data from [GH Archive](https://www.gharchive.org/) instead of Google Cloud
