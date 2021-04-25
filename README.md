# Neural_Network_Charity_Analysis

## Overview of the analysis

I used the features in the provided dataset to help create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

## Results

### Data Preprocessing
  - What variable(s) are considered the target(s) for your model?
    - The "IS_SUCCESSFUL" column is the targeted variable. 
  - What variable(s) are considered to be the features for your model?
    - All other columns with the exception of the targeted variable and our dropped columns. 
  - What variable(s) are neither targets nor features, and should be removed from the input data?
    - I dropped the "EIN" and "NAME" columns as they did not serve a purpose for my analysis. 


### Compiling, Training, and Evaluating the Model
  - How many neurons, layers, and activation functions did you select for your neural network model, and why?
    - In my most successful attempt I had input layer set to the length of X_train with 4 hidden layers; 1st layer with 100 neurons, 2nd with 50, 3rd with 25, and 4th with 10. I used the tanh activation function for each of the hidden layers and sigmoid for the output. 

    ![Deliverable3](https://github.com/RyanWhited/Neural_Network_Charity_Analysis/blob/main/images/deliverable3(1).jpg)
    
  - Were you able to achieve the target model performance?
    - With a goal of 75% accuracy I was only able to achieve 57%.
    ![Deliverable3](https://github.com/RyanWhited/Neural_Network_Charity_Analysis/blob/main/images/deliverable3.jpg)
    
  - What steps did you take to try and increase model performance?
    - First I increased the number of neurons to my original model, then I added more hidden layers, and finally experimented with changing the acitivation functions for my hidden and output layers. 

### Summary

After running numerous tests it seems that I could have some issues with the dataset provided that might need to be investigated. Another idea is to run an automated optimizer using keras tuner which I initially had performed but could not successfully translate the results for the best hyper parameters. 
