# deep-learning-challenge
# AlphabetSoup Charity Deep Learning Challenge
## Background
The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. With your knowledge of machine learning and neural networks, you’ll use the features in the provided dataset to 
create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

From Alphabet Soup’s business team, you have received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization, such as:

- **APPLICATION_TYPE:** Alphabet Soup application type
- **AFFILIATION:** Affiliated sector of industry
- **CLASSIFICATION:** Government organization classification
- **USE_CASE:** Use case for funding
- **ORGANIZATION:** Organization type
- **STATUS:** Active status
- **INCOME_AMT:** Income classification
- **SPECIAL_CONSIDERATIONS:** Special considerations for the application
- **ASK_AMT:** Funding amount requested
- **IS_SUCCESSFUL:** Was the money used effectively

## Step 1: Preprocess the Data

### 1.1 Upload Starter File to Google Colab
- Start by uploading the starter file to Google Colab.

### 1.2 Read in and Preprocess Data
- Read in the `charity_data.csv` to a Pandas DataFrame.
- Identify target(s) and feature(s) for your model.
- Drop the `EIN` and `NAME` columns.
- Determine the number of unique values for each column.
- For columns with more than 10 unique values, bin "rare" categorical variables together.
- Use `pd.get_dummies()` to encode categorical variables.
- Split the preprocessed data into features array (X) and target array (y).
- Scale the training and testing features datasets using `StandardScaler`.

## Step 2: Compile, Train, and Evaluate the Model

### 2.1 Create Neural Network Model
- Design a neural network model using TensorFlow and Keras.
- Assign the number of input features and nodes for each layer.
- Create the first hidden layer and choose an appropriate activation function.
- Add a second hidden layer if necessary.
- Create an output layer with an appropriate activation function.
- Check the structure of the model.

### 2.2 Compile and Train the Model
- Compile the model using appropriate settings.
- Train the model and create a callback to save weights every five epochs.
- Evaluate the model using the test data to determine loss and accuracy.
- Save and export results to an HDF5 file named `AlphabetSoupCharity.h5`.

## Step 3: Optimize the Model

### 3.1 Create Optimization Notebook
- Create a new Google Colab file named `AlphabetSoupCharity_Optimization.ipynb`.
- Import dependencies and read in `charity_data.csv` to a Pandas DataFrame.
- Preprocess the dataset as in Step 1, adjusting for any modifications from optimization.
- Design a neural network model, adjusting for modifications to achieve >75% accuracy.
- Save and export results to `AlphabetSoupCharity_Optimization.h5`.

## Step 4: Write a Report on the Neural Network Model

### 4.1 Overview of the Analysis
- Explain the purpose of the analysis.

### 4.2 Results

#### Data Preprocessing
- What variable(s) are the target(s) for your model?
- What variable(s) are the features for your model?
- What variable(s) should be removed from the input data because they are neither targets nor features?

#### Compiling, Training, and Evaluating the Model
- How many neurons, layers, and activation functions did you select for your neural network model, and why?
- Were you able to achieve the target model performance?
- What steps did you take in your attempts to increase model performance?

### 4.3 Summary
- Summarize the overall results of the deep learning model.
- Include a recommendation for how a different model could solve this classification problem.

## Step 5: Copy Files Into Your Repository

- Download Colab notebooks to your computer.
- Move them into your Deep Learning Challenge directory in your local repository.
- Push the added files to GitHub.

