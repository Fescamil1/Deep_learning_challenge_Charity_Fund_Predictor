# Deep_learning_challenge_Charity_Fund_Predictor
Deep Learning Homework: Charity Funding Predictor : will the Alphabet Soup–funded organization be successful?

## Instructions

### Step 1: Preprocess the data

Use Pandas and the Scikit-Learn’s `StandardScaler()`, to preprocess the dataset in order to compile, train, and evaluate the neural network model later in Step 2

Instructions to complete the preprocessing steps.

1. Read in the charity_data.csv to a Pandas DataFrame, and identify the following in the dataset:

- What variable(s) are considered the target(s) for the model?
- What variable(s) are considered the feature(s) for the model?

1. Drop the `EIN` and `NAME` columns.
2. Determine the number of unique values for each column.
3. For those columns that have more than 10 unique values, determine the number of data points for each unique value.
4. Use the number of data points for each unique value to pick a cutoff point to bin "rare" categorical variables together in a new value, `Other`, and then check if the binning was successful.
5. Use `pd.get_dummies()` to encode categorical variables

### Step 2: Compile, Train, and Evaluate the Model

Use TensorFlow to design a neural network, or deep learning model, to create a binary classification model that can predict if the organization will be successful based on the features in the dataset. Think about how many inputs there are before determining the number of neurons and layers in the model. Compile, train, and evaluate the binary classification model to calculate the model’s loss and accuracy.

1. Continue using the jupter notebook where you’ve already performed the preprocessing steps from Step 1.
2. Create a neural network model by assigning the number of input features and nodes for each layer using Tensorflow Keras.
3. Create the first hidden layer and choose an appropriate activation function.
4. If necessary, add a second hidden layer with an appropriate activation function.
5. Create an output layer with an appropriate activation function.
6. Check the structure of the model.
7. Compile and train the model.
8. Create a callback that saves the model's weights every 5 epochs.
9. Evaluate the model using the test data to determine the loss and accuracy.
10. Save and export your results to an HDF5 file, and name it `AlphabetSoupCharity.h5`.

### Step 3: Optimize the Model

Using your knowledge of TensorFlow, optimize your model in order to achieve a target predictive accuracy higher than 75%. If you can't achieve an accuracy higher than 75%, you'll need to make at least three attempts to do so.

Optimize your model in order to achieve a target predictive accuracy higher than 75% by using any or all of the following:

- Adjusting the input data to ensure that there are no variables or outliers that are causing confusion in the model, such as:
  - Dropping more or fewer columns.
  - Creating more bins for rare occurrences in columns.
  - Increasing or decreasing the number of values for each bin.
- Adding more neurons to a hidden layer.
- Adding more hidden layers.
- Using different activation functions for the hidden layers.
- Adding or reducing the number of epochs to the training regimen.

**NOTE**: You will not lose points if your model does not achieve target performance, as long as you make three attempts at optimizing the model in your jupyter notebook.

1. Create a new Jupyter Notebook file and name it `AlphabetSoupCharity_Optimzation.ipynb`.
2. Import your dependencies, and read in the `charity_data.csv` to a Pandas DataFrame.
3. Preprocess the dataset like you did in Step 1, taking into account any modifications to optimize the model.
4. Design a neural network model, taking into account any modifications that will optimize the model to achieve higher than 75% accuracy.
5. Save and export your results to an HDF5 file, and name it `AlphabetSoupCharity_Optimization.h5`.

### Step 4: Write a Report on the Neural Network Model

For this part of the Challenge, you’ll write a report on the performance of the deep learning model you created for AlphabetSoup.

The report should contain the following:

1. **Overview** of the analysis: Explain the purpose of this analysis.
2. **Results**: Using bulleted lists and images to support your answers, address the following questions.

- Data Preprocessing
  - What variable(s) are considered the target(s) for your model?
  - What variable(s) are considered to be the features for your model?
  - What variable(s) are neither targets nor features, and should be removed from the input data?
- Compiling, Training, and Evaluating the Model
  - How many neurons, layers, and activation functions did you select for your neural network model, and why?
  - Were you able to achieve the target model performance?
  - What steps did you take to try and increase model performance?

1. **Summary**: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and explain your recommendation.
