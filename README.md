# Neural Network Charity Analysis

## Overview
### Using machine learning and neural networks, use the features in the charity_data.csv to create a binary classifier that is capable of predicing whether applicants would be successful if funded by Alphabet Soup. This CSV contains more than 34,000 organizations that have received funding from Alphabet Soup over the years. This analysis of the charity_data.csv will be used to help the foundation predict where to make investments.

## Results

### Data Preprocessing

####  IS_SUCCESSFUL is the target for the model.

####  Features for the model:
##### * APPLICATION_TYPE
##### * AFFILIATION
##### * CLASSIFICATION
##### * USE_CASE
##### * ORGANIZATION
##### * ASK_AMT
##### * STATUS
##### * INCOME_AMT
##### * SPECIAL_CONSIDERATIONS

####  Variables that are neither targets/features and removed:
##### * EIN
##### * NAME

### Compiling, Training, and Evaluating the Model

#### Initial Analysis
##### * Hidden layer one: relu type - 8 neurons
##### * Hidden layer two: relu type - 5 neurons
##### * Activation: sigmoid
##### * Overall average accuracy: 72.90%
##### ![image](https://github.com/slafton/Neural_Network_Charity_Analysis/blob/main/images/First.png)
#### I started with a conservative number of neurons in my initial analysis as I planned to try increasing the number of neruons and hidden layers to improve accuarcy.

#### Improving Accuracy Attempts

#### Attempt 1
##### * Hidden layer one: relu type - 8 neurons
##### * Hidden layer two: relu type - 8 neurons
##### * Activation: sigmoid
##### * Overall average accuracy: 72.34%
##### ![image](https://github.com/slafton/Neural_Network_Charity_Analysis/blob/main/images/Second.png)
#### For the first attempt to increase accuaracy I increased the neurons in the second hidden layer to 8. The accuracy dropped however. 

#### Attempt 2
##### * Hidden layer one: relu type - 10 neurons
##### * Hidden layer two: relu type - 10 neurons
##### * Activation: sigmoid
##### * Overall average accuracy: 72.83%
##### ![image](https://github.com/slafton/Neural_Network_Charity_Analysis/blob/main/images/Third.png)
#### For the second attempt to increase accuracy I increased the number of neurons in both the first and second hidden layers to 10. This accuracy was better than the last attempt but still a little less than the initial analysis. 

#### Attempt 3
##### * Hidden layer one: tahn type - 10 neurons
##### * Hidden layer two: relu type - 8 neurons
##### * Hidden layer three: sigmoid type - 6 neurons
##### * Activation: sigmoid
##### * Overall average accuracy: 72.69%
##### ![image](https://github.com/slafton/Neural_Network_Charity_Analysis/blob/main/images/Fourth.png)
#### For the third attempt to increase accuracy I added a third hidden layer with 6 neurons and decreased the neurons in the second layer to 8. Ther accuracy dropped from the previous attempt.

## Summary
### More analysis could be done with increased hidden layers and neurons. While the initial analysis achieved the best overal accuracy. The attempt with two hidden layers with ten neurons was close behind it so it may be possible with more hidding layers and higher numbers of neurons to achieve the goal of 75% accuracy that has yet to be achieved.

### A Random Forest Classifier could be an alternative model to try. The Random Forest is able to perform binary classification and handle large data sets. It aggregates the results from randomly selected subsets of the training set to decide the final class of the test object. 
