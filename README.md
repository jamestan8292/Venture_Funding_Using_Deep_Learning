# Venture_Funding_Using_Deep_Learning

## Overview of the Classifier

This deep learning learning classifier is developed under hypothetical venture capital firm, Alphabet Soup. Alphabet Soup’s business team receives many funding applications from startups every day. This team wanted an application to help them create a model that predicts whether applicants will be successful if funded by Alphabet Soup.

Alpahbet Soup has a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Using machine learning and neural networks, the features in the provided dataset is used to create a binary classifier model that will predict whether an applicant will become a successful business. The CSV file contains a variety of information about these businesses, including whether or not they ultimately became successful.

Tensorflow with Keras is used for deep learning process. Four approaches, by varying the number of epochs, layers and nodes were used to optimize the original model. The models are saved in h5 files.


## Results

After pre-processing, the dataframe has 116 features and one target. Five neural network models were tested. The following were the accuracies achieved for the five models:

* Original Model: Two hidden layers, with the first layer with the number of nodes equals to half the number of features, and the second layer having half the number of nodes of the first layer. The RELU activation function is used for the hidden layers. The model was run for 50 epochs.
  * Accuracy = 72.7%

* Alternate Model 1: Same parameters as the Original Model, with the model run for 100 epochs.
  * Accuracy = 73.0%

* Alternate Model 2: Two hidden layers, with the first layer with the number of nodes equals to twice the number of features, and the second layer having twice the number of nodes of the first layer. The model was run for 50 epochs.
  * Accuracy = 73.0%

* Alternate Model 3: Same parameters as Alternate Model 2, with the SELU activation function used for the hidden layers in place of the RELU function. The model was run for 50 epochs.
  * Accuracy = 72.9%

* Alternate Model 4: Same parameters as the Original Model, with one additional hidden layer. The model was run for 50 epochs.
  * Accuracy = 73.0%


## Observations with this Dataset

1. For the same model, increasing the number of epochs marginally improved the accuracy (Original Model vs Alternate Model 1)

2. Increasing the number of nodes only show a marginal improvement in accuracy (Alternate Model 2 vs Original Model), and no improvement in accuracy with higher number of epochs versus increasing number of nodes.

3. The RELU activation function performed marginally better than the SELU function (Alternate Model 2 vs Alternate Model 3)

4. Adding an additiona layer showed a marginal accuracy improvement (Alternate Model 4 vs Original Model)

---

## Technologies

This analysis is written for use with Jupyter Lab. It uses the following packages:. It uses the following packages:

* [Pandas](https://github.com/pandas-dev/pandas)
* [sklearn](https://scikit-learn.org)
* [TensorFlow](https://www.tensorflow.org)


---

## Usage

In Windows GitBash or Mac Terminal app, enter "Jupyter Lab". Then open and run "venture_funding_with_deep_learning.ipynb".

The "applicants_data.csv" file must be in a sub-folder "Resources".


---

## Contributors

This application is written by James Tan, with code snippets provided UBC Extension.

---

## License

MIT.
