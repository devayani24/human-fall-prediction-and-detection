# human-fall-prediction-and-detection
## 1.1 CAUSES OF FALL IN PEOPLE
#### Falls are usually caused by an interaction of a number of risk factors. The more risk factors you have, the greater your risk of falling. Falls prevention is about recognizing,
#### and where possible, taking action to reduce the risk.
## 1.2 AIM
#### To improve the health, function, and quality of life by predicting the fall of peoples.
## 1.3 OBJECTIVE
#### Increase the proportion of old people, bed ridden patients who are up to date on a core set of clinical preventive services.
#### To predict the anticipated fall and give alert to the caretaker and to protect the user in case of a fall.
## 1.4IMPORT THE NECESSARY LIBRARIES
#### A library is a collection of non-volatile resources used by computer programs, often for software development. The major library that is used for machine learning is
#### pandas (used to read the dataset), numpy (used to perform basic array operations),standardscaler(used to bring all data in the same scale), labelEncoder and so on.
#### Predominantly, tensorflow-Keras is used to build the CNN model.

## 1.5 BALANCING THE DATA
#### It is necessary to observe whether our data is balanced or unbalanced. If it is the case 2, our model will over fit towards the label which has an enormous data when
#### compared to other labels and ultimately produce the wrong accuracy.
## 1.6 STANDARDIZATION
#### Data standardization is about making sure that data is internally consistent; that is, each data type has the same content and format. Standardized values are useful for
#### tracking data that isn't easy to compare otherwise.
## 1.7 FRAME PREPARATION
#### In order to feed the data into our neural network, it must be reshaped in such a way that input must be time series for atleast 0.4 sec to predict the action.  
![image](https://user-images.githubusercontent.com/76246283/119127787-5de05680-ba52-11eb-949c-a93a79cab995.png)

## 1.8 SPLITTING OF TRAINING AND TESTING DATA
#### Before we fit our data in our model, splitting training (80%) and testing data (20%) is done to evaluate the results.
#### Training set—a subset to train a model.
#### Test set—a subset to test the trained model.
#### Here we split the data’s into 80% for training and 20% for testing.
## MODEL BUILDING
### 2D CNN
#### Layer used-  Conv2D, FullyConnected layer

#### Activation function used- Relu  and Softmax 

#### Optimisation used- Adam optimizer  

#### Loss function used- sparse categorical crossentropy 

#### Droput layer is used to reduce the overfit
![image](https://user-images.githubusercontent.com/76246283/119127824-6a64af00-ba52-11eb-97e5-b11616467d06.png)



## MODEL ACCURACY AND LOSS
#### If we plot the evolution of the two error scores as training sets change, we end up with two curves. These are called learning curves. In a nutshell, a learning
#### curve shows how error changes as the weight increases. It is plotted for 10 epochs.
![image](https://user-images.githubusercontent.com/76246283/119127717-486b2c80-ba52-11eb-8fcc-d01cb7c0af4d.png)
![image](https://user-images.githubusercontent.com/76246283/119127731-4dc87700-ba52-11eb-948b-260b1208c489.png)

## CONFUSION MATRIX
#### A confusion matrix is a table that is often used to describe the performance of a classification model on a set of test data for which the true values are known.
#### The confusion matrix itself is relatively simple to understand, but the related terminology can be confusing.
![image](https://user-images.githubusercontent.com/76246283/119127665-38ebe380-ba52-11eb-9497-1e596318d85e.png)

