# Neural_Network_Charity_Analysis

## Overview of the analysis: 
In this analysis we are examining different organizations that received funding from Alphabet Soup and using the dataset to build a neural network to predict where the company can make investments. We’ll be using Keras to build a basic neural network to determine where the company can make successful investments in the future.

## Results: 

**Data Preprocessing**

**What variable(s) are considered the target(s) for your model?**
The target for this model are the successful organizations that completed their funding projects.

**What variable(s) are considered to be the features for your model?**
The features for this model would be the: application type, affiliation, classification, use case, organization, income amount, and ask amount. 

**What variable(s) are neither targets nor features, and should be removed from the input data?**
Variables that are neither and were removed from data tables via preprocessing were: EIN, name, status, and special considerations.

**Compiling, Training, and Evaluating the Model**

**How many neurons, layers, and activation functions did you select for your neural network model, and why?**
There were two layers with 80 neurons for the first layer and 30 for the second layer, since the input variables is about 40 variables, we selected 2 times the amount of neurons for the first layer. The two layers used the activation layer RELU and the output layer had the activation sigmoid layer. 

**Were you able to achieve the target model performance?**
No, the target model performance did not exceed 75%, it fell a bit short.

![optimized_results](https://github.com/vanessaneang/Neural_Network_Charity_Analysis/blob/main/Resources/optimized_results.png)


**What steps did you take to try and increase model performance?**
I tried to exclude two more columns that were not necessary for the model learning to decrease the workload the for the neural network algorithm. In addition to this I tried to increase the number of neurons to 160 for the first layer in hopes to increase the accuracy. Lastly, I added an additional layer with 5 neurons to see if it would increase the overall accuracy.
![optimized_code](https://github.com/vanessaneang/Neural_Network_Charity_Analysis/blob/main/Resources/optimized_neural.png)


## Summary: 
The result of the deep learning model was fairly successful with both models having an accuracy rate of 70%, this indicates that it can predict successful organizations to invest in about 2/3rds of the time. Since there are multiple inputs for the model with only one output needed it would be easier if we could use a logistic regression model or another supervised machine learning model. Not only would this code outperform the neural network in processing time it would either give the same accuracy rate or be more optimal for the model.

