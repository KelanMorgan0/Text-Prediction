# Text-Prediction

## Text Prediction
This repository contains a [Jupyter](https://jupyter.org/) Notebook With the means to run a machine learning script to predict the next character in a sentence

**Data**
the data was recieved from [Sentiment140 dataset with 1.6 million tweets](https://www.kaggle.com/datasets/kazanova/sentiment140) which gives a data set containing the following columns:
- **Target:** this column contains the sentiment value
- **Ids:** this column contains the id of the tweet
- **Date:** this column has the date of the entry
- **flag:** this column has the query of the entry
- **User:** this column has the username of the entry
- **Text:** this column has the text from the tweet

The data is taken in using pandas and stored in a variable

**Pre-Processing**

- Remove all columns except for "Text"
- Reduce data size to 50,000 rows
- remove all hashtags and mentions
- remove all urls
- ensure only letters, numbers and punctuation symbols are left

**RNN**

the characters in the text are converted to numerical data, this is for the models understanding of the characters

The model is then trained to an accuracy of ~50% over 5 Epochs, this may be able to be raised with more data used and more Epochs, however due to time constraints, this was not possible

**Prediction**

Using an Entered String, The model attempts to predict the next character a number of times inserted to the function