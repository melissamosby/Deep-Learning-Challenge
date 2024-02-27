## Deep-Learning-Challenge
Module 21

## Overview 
Alphabet Soup that wants to use a tool that can help it select the applicants for funding with the best chance of success in their ventures. Using machine learning and neural networks, we use the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

## Results
* Data Preprocessing
	* What variable(s) are the target(s) for your model?
	Our target is the "y" which is the "IS_SUCCESSFUL" column

	* What variable(s) are the features for your model?
	Our features is the "X" which is everything but the "IS_SUCCESSFUL" column
as: "APPLICATION_TYPE" , "AFFILIATION", "CLASSIFICATION", "USE_CASE", "ORGANIZATION", "STATUS", "INCOME_AMT", "SPECIAL_CONSIDERATIONS", "ASK_AMT"

	* What variable(s) should be removed from the input data because they are neither targets nor features?
	"EIN & "NAME" were removed from variables, since they are neither targets nor features.

* Compiling, Training, and Evaluating the Model
	* How many neurons, layers, and activation functions did you select for your neural network model, and why?
 	There are four layers, three input layers, two hidden layers and one output layers. In addition, there are 43+80+30+1=154 neurons. There are two activitation functions. The relu function was used because X is non linear relationship. For the output, Sigmoid was used because the result is two value classifications. 

  * Were you able to achieve the target model performance? 
	Yes, the target model performance accuracy was 0.7402.

  * What steps did you take in your attempts to increase model performance? There are four ways to increase the performance:
	1. Increase layer of neural network and check if performance is getting better.
	2. Adjusting the neural unit number. Using too few neural numbers may lead to underfitting. On other hand, using too many neural numbers may result in overfitting.
	3. You can change the activitation function, for hidden layer use `relu` and for classification we can use `Sigmoid`, for multiple classification use `softmax`, for regression use `linear`.
	4. Increase the number of epochs.


## Summary
* For this model, the loss is 56% and accuracy is 72% after 100 epoch runs. When the neural network model is running, the loss should drop and approach zero, at the same time the accuracy should rise. So, 72% of accuracy is good enough, but 56% of loss is not good and far away from having a successful model. We have to retrain the model to lower the loss using the techniques listed above. 
