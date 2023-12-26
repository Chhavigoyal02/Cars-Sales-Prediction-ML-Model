# Cars-Sales-Prediction-ML-Model

*PROBLEM STATEMENT*
You are working as a car salesman and you would like to develop a model to predict the total dollar amount that customers are willing to pay given the following attributes: 
- Customer Name
- Customer e-mail
- Country
- Gender
- Age
- Annual Salary 
- Credit Card Debt 
- Net Worth 

The model should predict: 
- Car Purchase Amount


PROJECT OVERVIEW:
-- First of all,we need to check whether it is regression task or classifiction task...
    It is a regression task as we have to predict a continuous value i.e. Car Purchase Amount.
-- Here,we are going to use regression and Artificial Neural Networks to get this task done.

STEPS TAKEN:

So,here are the step I followed in this problem statement:

--> Step-0: Importing the libraries like numpy(for basic calculations),pandas(for dataframes references),matplotlib(for graph plotting) and seaborn(for visualising the data)

--> Step-1: Load the dataset(here car sales prediction) which is csv file.For reading this csv fle we can use pandas.

--> Step-2: Visualise the data (by seaborn library) means plotting grpahs between several features and checking the relationship between dependent and independent variables.

--> Step-3: Now we create training and testing dataset and do data preprocessing.So,first drop unnnecessary columns like costumer name, costumer email and country and rest of the columns get stored into X. also,the dependent variable (here car purchasing amount) get stored into y.
*And for data cleaning, normalisation should be done. Normalization in machine learning is the process of translating data into the range [0, 1] (or any other       range) or simply transforming data onto the unit sphere. Here, we use MinMaxScaler for normalisation.Without normalisation, functionality of model will be          distorted.

--> Step-4: Training the Model. First, call train_test_split function and split the whole dataset into four parts - X_train, X_test, y_train and y_test.
*Now,I am using Keras library for executing Artificial Neural Networks(ANNs).Keras is a Python library that is designed specifically for developing the neural       networks for ML models. It can run on top of Theano and TensorFlow to train neural networks. 
*So, create two hidden layers by giving 25 neurons and activation function as ReLu function(Rectified Linear Unit function).
*Create 1 output layer which include 1 neuron and activation function as linear function.
*Here, I gave numner of epochs as 20. An epoch is when all the training data is used at once and is defined as the total number of iterations of all the training    data in one cycle for training the machine learning model. 

--> Step-5: Evaluating the Model.Plot the graph of Model Loss Progression During Training/Validation between Training and Validation Losses and Number of Epochs.
hence,find out the y_predict by X_test.
