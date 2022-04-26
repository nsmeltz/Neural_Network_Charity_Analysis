# Neural Network Charity Analysis

## **Overview** 
The purpose of this analysis is to apply deep neural network machine learnign algorithms to determine whether or not an organization that is funded by AlphabetSoup is successfull 

## **Results**
  - Data Preprocessing
    - What variable(s) are considered the target(s) for your model?                         
      The target for this model is prediction whether or not the charity is successful.
      ![targets](https://github.com/nsmeltz/Neural_Network_Charity_Analysis/blob/9f803b99525d9cd329d43ae2489345b9cf3491d7/Images/target.jpg)
      
    - What variable(s) are considered to be the features for your model?                                     
    ![features](https://github.com/nsmeltz/Neural_Network_Charity_Analysis/blob/9f803b99525d9cd329d43ae2489345b9cf3491d7/Images/features.jpg)
   
    - What variable(s) are neither targets nor features, and should be removed from the input data?                           
    ![delete](https://github.com/nsmeltz/Neural_Network_Charity_Analysis/blob/9f803b99525d9cd329d43ae2489345b9cf3491d7/Images/neither.jpg)
    
  - Compiling, Training, and Evaluating the Model
    - How many neurons, layers, and activation functions did you select for your neural network model, and why?
      There are 38 input features so I added 2-3 times as many neurons to each of the hidden layers (80 and 30 respectively)
      I used the relu function for the hidden layers because it is best for non-linear data.
      I used the sigmoid function for the output layer because sigmoid normalizes the output to a probablility between 0 and 1.
      
    - Were you able to achieve the target model performance?
      No
      
    - What steps did you take to try and increase model performance?
      I added another layer with 50 neurons 
      I increased the original layers to 100 and 80 neurons
      I decreased the number of classifications and application types by expanding the bins to try to simplify the input data to the neural network
      
## **Summary**

The original configuration of this model had an accuracy of ~72.63 % and a loss of 0.5563
The "optimized" configuration had and accuracy fo 72.26% and a loss of 0.5800

The changes that I made did not make any significance in the outcome of the model. I also played around with the automated optimizer and it couldn't come up with a set of hyperparameters that resulted in a model with much better than a ~72% accuracy. This leads me to think that a different machine learning algorithm may be better for this type of classification problem like a k means clustering with the features that are considered most important to the outcome of whether or not the organization was successful with their funding. 
