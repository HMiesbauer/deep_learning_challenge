# deep_learning_challenge#

#Overview#<br>
The purpose of this analysis was to create a binary classifier that would be effective at predicting venture success based on funding

#Results# <br>

##Data Preprocessing##
*What variable(s) are the target(s) for your model?
    *IS_SUCCESSFUL is the target for the model
*What variable(s) are the features for your model?
    *APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, INCOME_AMT, ASK_AMT
*What variable(s) should be removed from the input data because they are neither targets nor features?
    *Intially, only a few features were removed from the input data: NAME and EIN along with the target IS_SUCCESSFUL
    *Ultimately, the model only retained six features and the one target.

##Compiling, Training, and Evaluating the Model##
*How many neurons, layers, and activation functions did you select for your neural network model, and why?
    *I selected very few at the end because I was trying to optimize the model. I felt the features where what was causing the model to be less effective than the target. I did train one model with an activation function softmax which significantly decreased the accuracy. Overall, I chose the activation function sigmoid produced the most effective model.
*Were you able to achieve the target model performance?
    *I was not able to achieve the target model performance. My best model has a 73% effectiveness.
*What steps did you take in your attempts to increase model performance?
    *I removed features, I increased epochs, I increased layers and none of those efforts improved the model beyond 73% effectiveness.
    
![Confusion Matrix Model 1](https://github.com/HMiesbauer/deep_learning_challenge/assets/150979374/25250545-c1fc-455e-b12e-0b9fde66bd0f)
![Confusion Matrix Model 3](https://github.com/HMiesbauer/deep_learning_challenge/assets/150979374/869ff9cd-4714-4651-a2cd-f3704e9209d0)
  
#Summary#

*Overall, the intial model produced satisfactory results even though it didn't achieve target performance. I could have used a Gradient Booster Classifier which would have included feature importance scores. This would have allowed me to optimize the model with the higher feature scores thus improving the overall model efficiency.

![SHAP Summary Plot](https://github.com/HMiesbauer/deep_learning_challenge/assets/150979374/33afca65-6719-490a-b2f6-788c8d201afa)
