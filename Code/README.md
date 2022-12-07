# Code

Support Vector Machine (SVM) and Artificial Neural Network (ANN) mushroom edibility classification in R (RMarkdown).

Visual exploration of the dataset was done using the ggplot2 library. This library allows the visualization of the character variables using scatterplot graphs.

The two models are trained and tested using a processed version of the mushroom dataset. Missing values are dealt with by converting them from a question mark character to u (unknown) character. The dataset contains only categorical variables so they are converted to numerical variables using One-Hot-Encoding. This way the models can actually use the dataset and extract information for classification.

A few models for both algorithms are trained with different parameters to observe if there is a difference in performance. K-fold cross validation is used on the best performing SVM model to have greater confidence that the model has not been overfitted. The optimal parameters for the ANN is found using grid search. This optimal model is then trained and tested for performance measure.