    # Introduction to K-Fold Cross-Validation
    
    
    cross Validation is a technique which is used for assessing the performance of machiene learning models..The problem with machiene learning models is that you won't get to know how well a model performs until you test its performance on an independent data set(the data set which was not used for training the machine learning model).You want to used this technique to estimate how accurate the predictions your model will give in practice.When you are given a machine learning problem, you will be given two type of data sets — known data (training data set) and unknown data (test data set). By using cross validation, you would be “testing” your machine learning model in the “training” phase to check for overfitting and to get an idea about how your machine learning model will generalize to independent data, which is the test data set given in the problem.
    There are many variation' method,and the most commomnly used one is known as 'k fold cross-validation'.
    
    k-fold cross-validation is one of the most commomnly used model evaluation methods.
    
    ## Steps in ‘k’ fold cross-validation 
    
    * In this method, the training dataset will be split into multiple ‘k’ smaller parts/sets. Hence the name ‘k’-fold.  
* The current training dataset would now be divided into ‘k’ parts, out of which one dataset is left out and the remaining ‘k-1’ datasets are used to train the model.  
* This is done multiple number of times. The number of times that it has to be done is mentioned by the user in the code.  
* The one that was kept out of the training is used as a ‘validation dataset’. This can be used to tune hyperparameters and see how the model performs and change the values accordingly, to yield better results.  
* Even though the size of the dataset isn’t reduced considerably, it was reduced to a certain extent. This method also makes sure that the model remains robust and generalizes well on the data. 

## How is the value of ‘k’ decided? 
 It is a trial and error method in which the value is chosen. Usually it is taken as 10 which is completely arbitrary.This depends on the data in hand. A large value for ‘k’ indicates less bias, and high variance. Also, this means more data samples can be used to give a better, and precise outcomes.
 
 
 ## Applications of Cross Validation
 
 The cross validation technique can be used to compare the performance of different machine learning models on the same data set. To understand this point better, consider the following example.
 * It ‘validates’ the performance of your model on multiple ‘folds’ of your data.
 * It can balance out the predicted features’ classes if you are dealing with an unbalanced dataset.
 * Because of 1 and 3 it gives you a more stable answer as to how your model performs on that data.
 
 ## Variations of cross-validation  :
 There are variations to cross validations, and they are used in relevant situation. Others are:
 * Leave one out cross validation 
* Leave ‘p’ out cross validation  
* ‘k’ fold cross validation 
* Holdout method 
