# Deep_learning_challenge_Charity_Fund_Predictor
Deep Learning Homework: Charity Funding Predictor purpose/goal is to predict if the Alphabet Soup–funded organization will be successful.

### Preprocess the data

The target variable for the model will be "IS_SUCCESSFUL". This column has values of 1 and 0 which helps us determine if the charity fund is successful (1) or not successful(0).  After columns "EIN" and "Name" are dropped, the remaining columns are features for the model. 

### Compile, Train, and Evaluate the Model

Use TensorFlow to design a neural network, or deep learning model, to create a binary classification model that can predict if the organization will be successful based on the features in the dataset. Compile, train, and evaluate the binary classification model to calculate the model’s loss and accuracy.

**Run 1** : Use neural network model with 2 hidden layers. 1st layer with 80 nodes and second layer with 30. Using 100 epochs. 

​	This model resulted in a Loss: 0.5574843883514404 and Accuracy of 0.7316617965698242. Although this is below the desired target of .75 it is close. 

**Run 2:**  Use neural network model with 3 hidden layers. 1st layer with 60 nodes, second layer with 40 and third layer with 20. Using 100 epochs. 

​	This model resulted in a Loss: 0.5652271509170532 and of Accuracy: 0.7327113747596741. Did not find any have any significant improvement in accuracy. Even noticed a slight increase in loss. 

**Run 3:** Use neural network model with 4 hidden layers distributed in the following way 80, 50, 30, and 5. Using 100 epochs.  Total parameters increased dramatically from the prior runs. 

​	This model resulted in Loss of 0.5677768588066101 and Accuracy dropped to  0.7274635434150696. Adding more hidden layers did not result in improved accuracy. Will attempt to redo Run#2 with increased epochs. 

**Run 4:** Use neural network model with 3 hidden layers. 1st layer with 60 nodes, second layer with 40 and third layer with 20. Using 200 epochs.

​	This model resulted in a of Loss: 0.5851432681083679 and Accuracy of 0.7336443066596985. This model resulted in the highest accuracy. However, it did not achieve the desired accuracy of 75%. 

All saved in HDF5 file named AlphabetSoupCharity.h5



 **Summary:**  Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and explain your recommendation.
