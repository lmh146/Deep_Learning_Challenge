# Deep_Learning_Challenge

## Analysis Report

### Data Processing
In the data processing section the targeted variable in this model is addressing if the applicant applying for funding was successful. Therefore, the "IS_SUCCESFUL" column is our target variable.

In terms of features, APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, and ASK_AMT are all the features used in the model. Following the one-hot encoding, APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, and SPECIAL_CONSIDERATIONS are further broken down into additional features based on their unique values.

EIN and NAME columns are neither targets nor features as they are identifiers. This means each row, particularly in the EIN column, will have a unique number and will thusly not be beneficial to the modeling.

### Compiling, Training, and Evaluating the Model
In the end, I chose 3 layers with 100, 80, and 30 neurons in a descending order. With activation functions of relu and sigmoid on the output. I came to this level through trial and error. My accuracy wasn't changing significantly, so I took my slightly higher accuracy and tried adjust it more but nothing resulted from most of the attempts. I did see a significant decrease in accuracy when I had relu activation in the output layer and sigmoid activation in the hidden layers.

Unfortunately I was not able to achieve the target performance.
To try and improve the performance I increased the number of neurons in the layers, increased the number of hidden layers, and tested different activation functions. In the future I could do better with decreasing the noisy features.

### Summary
This model looks to predict the success of candidates looking for funding. While the run of the model here was unsuccessful and further analysis would be needed to completely determine issues, but the use of the tanh activation function in future as well as additional neural networks to give the data more specificity when running through the layers. Using a logistical regression may also be useful as it also works well for binary classification and could help to simplify the process.
