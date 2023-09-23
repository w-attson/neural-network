## Venture Funding with Deep Learning Project

This project creates a model that predicts whether applicants will be successful if back by a venture fund.
The data is a CSV that contains more than 34,000 organizations that have received funding over the years. The CSV file contains a variety of information about the businesses, including whether or not they ultimately became successful.

## Steps in the Neural Network Project

* Read the applicants_data.csv file into a Pandas DataFrame.
  * Review the DataFrame, looking for categorical variables that will need to be encoded, as well as columns that could eventually define the features and target variables.


* Drop the “EIN” (Employer Identification Number) and “NAME” columns from the DataFrame, because they are not relevant to the binary classification model.


* Encode the dataset’s categorical variables using OneHotEncoder, and then place the encoded variables into a new DataFrame.


* Add the original DataFrame’s numerical variables to the DataFrame containing the encoded variables and concat the dataframes.


* Using the preprocessed data, create the features (X) and target (y) datasets. The target dataset should be defined by the preprocessed DataFrame column “IS_SUCCESSFUL”. The remaining columns should define the features dataset.


* Split the features and target sets into training and testing datasets.

* Use scikit-learn's StandardScaler to scale the features data.

* Create a deep neural network by assigning the number of input features, the number of layers, and the number of neurons on each layer using Tensorflow’s Keras.

* Compile and fit the model using the binary_crossentropy loss function, the adam optimizer, and the accuracy evaluation metric.

* Evaluate the model using the test data to determine the model’s loss and accuracy.

* Save and export your model to an HDF5 file, and name the file AlphabetSoup.h5.

## Optimize the Neural Network Model

* Define at least three new deep neural network models.

  * Adjust the input data by dropping different features columns to ensure that no variables or outliers confuse the model, Examples:.
  
  * Add more neurons (nodes) to a hidden layer.
  
  * Add more hidden layers.
  
  * Use different activation functions for the hidden layers.
  
  * Add to or reduce the number of epochs in the training regimen.

* After finishing the modelling, display the accuracy scores achieved by each model, and compare the results.

* Save each of the models as an HDF5 file.