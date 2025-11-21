# Data-Mining-Final-Project

# First step: Dataset

We started by pulling stock data from yahoo finance and altering the dataframes into a more standard labling scheme. We then added our target (if the close goes up the next day or not). From this, we made two datasets. 1 - the ohlcv and our target. 2 - the ohvcv, out target, and calculated indicators (moving average, RSI)

# Second set: Models

Using scikit learn, we were able to quickly train and evaluate the models we decided on. This included decision tree, random forest, logistic regression, SVM, and MLP. From this we found that all the models were getting and accuracy of .52 and an recall of 1. This strongly indicated to us that the models were just guessing the stock would go up every time. From here we implemented fix after fix to try and get the models to predict properly.

# Fix 1: Normalization

Given that stocks have different prices and price ranges, we thought that normalization would help. We added normalization to a few models we thought it would help.

Unfortunatly, there was no improvement.

# Fix 2: Stationary

So given that we are using multiple stocks which do cost different things, we needed a way to standardize what values we were looking at. This was also an issue between the train and test sets and generally, the test set would be higher in absolute values, so Normalization didn't help.

This has not been implemented yet but I will work on it.
