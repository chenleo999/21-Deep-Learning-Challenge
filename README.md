# 21-Deep-Learning-Challenge

completed by Li Chen 6/8/2024

description:
Alphabet Soup, a nonp-profit foundation needs to filter their applicants for the best chance of success.  Use machine learning and neural networks knowledge, I have built a binary classifier for predicting applicants' potential success, which shall assit Alphabe Soup in better reward from their funding.

Dataset- a csv file containg 34000+ historic records

Pre-process
    1. read csv into Pandas DataFrame and remove non-benificial columns
    2. check unique value for columns, pick cut-off and combine rare values to 'Other'
    3. turn categorical variables to numeric
    4. split into feature X and target y arrays, then into training and testing datasets
    5. standard scale both datasets, fit training data, transform

Compile, Train, Evaluate Model
    6. build TensorFlow neural networks model, assign input feature and node numbers for each layer and activation function
    7. check model structure, compile and train
    8. evaluate model with test data, export HDF5

Result 1: Accuracy is 72.9%, less then 75%, the model needs optimization.

Optimization:
    1. Dropping fewer columns, keep "NAME"
    2. Increase number of values "CLASSIFICATION" by change cut-off from 1000 to 100
    3. Adjust number of nodes in hidden layers

Result 2: Accuracy is 78.9%, pass !
