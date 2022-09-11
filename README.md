# Venture_Funding_Using_Deep_Learning

## Overview of the Classifier

This deep learning learning classifier is developed under hypothetical venture capital firm, Alphabet Soup. Alphabet Soup’s business team receives many funding applications from startups every day. This team wanted an application to help them create a model that predicts whether applicants will be successful if funded by Alphabet Soup.

Alpahbet Soup has a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Using machine learning and neural networks, the features in the provided dataset is used to create a binary classifier model that will predict whether an applicant will become a successful business. The CSV file contains a variety of information about these businesses, including whether or not they ultimately became successful.

Tensorflow with Keras is used for deep learning process. Four approaches, by varying the number of epochs, layers and nodes were used to optimize the original model. The models are saved in h5 files.


## Results

After pre-processing, the dataframe has 116 features and one target. Five neural network models were tested. The following were the accuracies achieved for the five models:

* Original Model: Two hidden layers, with the first layer with the number of nodes equals to half the number of features, and the second layer having half the number of nodes of the first layer. The RELU activation function is used for the hidden layers. The model was run for 50 epochs.
  * Accuracy = 73.0%

* Alternate Model 1: One hidden layer, with the hidden layer with the number of nodes equals to half the number of features. The model run for 50 epochs.
  * Accuracy = 73.1%

* Alternate Model 2: One hidden layer, with the hidden layer with the number of nodes equals to twice the number of features. The model was run for 50 epochs.
  * Accuracy = 73.2%

* Alternate Model 3: Same parameters as Alternate Model 2, with the SELU activation function used for the hidden layers in place of the RELU function. The model was run for 50 epochs.
  * Accuracy = 73.0%



## Observations with this Dataset

1. Using one instead of two layers, with the same 50 epochs, improved the accuracy (Original Model vs Alternate Model 1). Having more than one layer in this case may be a sign of oversampling.

2. Increasing the number of nodes showed a little improvement in accuracy (Alternate Model 2 vs Alternate Model 1). Alternate Model 1 run faster because it has less number of nodes. 

3. The RELU activation function performed slightly better than the SELU function (Alternate Model 2 vs Alternate Model 3).


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
