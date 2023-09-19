# Report 
For this part of the assignment, you’ll write a report on the performance of the deep learning model you created for Alphabet Soup.

The report should contain the following:

1. Overview of the analysis: Explain the purpose of this analysis.

2. Results: Using bulleted lists and images to support your answers, address the following questions:

## Data Preprocessing

1. What variable(s) are the target(s) for your model?
The target variable is the 'IS_SUCCESSFUL' column from application_df
2. What variable(s) are the features for your model?
The feature variables are every other column from application_df --> this was defined by dropping the 'IS_SUCCESSFUL' column from the original dataframe
3. What variable(s) should be removed from the input data because they are neither targets nor features?
Both 'EIN' and 'NAME' columns were dropped/removed, because they were neither targets nor features for the dataset.

## Compiling, Training, and Evaluating the Model

1. How many neurons, layers, and activation functions did you select for your neural network model, and why?
ATTEMPT 1
The first attempt (Models/AlphabetSoupCharity1.h5) resulted in an accuracy score of 72.8%. This was the highest accuracy score of the three models. This means that 72.8% of the model’s predicted values align with the dataset’s true values.

The hyperparameters used were:

layers = 2
layer1 = 9 neurons : activation function = ‘relu’
layer2 = 18 neurons : activation function = ‘relu'
epochs = 100

ATTEMPT 2
For my second attempt. This attempt resulted in an accuracy score of 72.8%. This means that 72.8% of the model’s predicted values align with the dataset’s true values.

The hyperparameters used were:

layers = 2
layer1 = 10 neurons : activation function = ‘relu’
layer2 = 10 neurons : activation function = ‘relu’

epochs = 100

ATTEMPT 3
2 layer and changed the activation function for layers 1 and 2. This attempt resulted in an accuracy score of 73.4%. This means that 73.4% of the model’s predicted values align with the dataset’s true values.

The hyperparameters used were:

layers = 2
layer1 = 10 neurons : activation function = ‘tanh’
layer2 = 19 neurons : activation function = ‘relu’

epochs = 100
2. Were you able to achieve the target model performance?
I was not able to achieve the 75% model accuracy target
3. What steps did you take in your attempts to increase model performance?
I added more layers, removed more columns, added additional hidden nodes, and switched up the activation functions associated with each layer in an attempt to achieve higher model accuracy.

## Summary
Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and then explain your recommendation.

Overall, the deep learning model was around 73% accurate in predicting the classification problem. Using a model with greater correlation between input and output would likely result in higher prediction accuracy. This could be achieved by doing additional data cleanup up front, as well as by using a model with different activation functions and iterating until higher accuracy is reached.