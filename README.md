Neural_Network_Charity_Analysis

Overview of the analysis: 

Neural networks are an advanced form of machine learning that recognizes patterns and features in input data and provides a clear quantitative output.  Given a dataset of charitable organizations, the purpose of this analysis is to create a binary classifier that can predict whether applicants will be successful when provided with funding. The project delivers a neural network model that has been preprocessed, compiled, trained, evaluated, and optimized.

Results:

Data Preprocessing

What variable(s) are considered the target(s) for your model?
The target, or predicted outcome, for this model is the “Is Successful” column.

What variable(s) are considered to be the features for your model?
The features, or variables used to make the prediction, are all the remaining columns except for
the “Is Successful” and dropped columns.

What variable(s) are neither targets nor features, and should be removed from the input data?
The variables considered to be neither a target nor a feature were the “EIN” and “Name” columns.

![image](https://user-images.githubusercontent.com/100803302/178154442-46d57b65-3fc9-48c1-a919-3494f6fed14f.png)

Compiling, Training, and Evaluating the Model

How many neurons, layers, and activation functions did you select for your neural network model, and why?
For deliverable 2, the model was defined with 40 neurons in a first layer, 20 neurons in a second layer, and the activation function “ReLu.” For this initial model the number of neurons and layers was selected to establish a baseline model that might reach our desired level of performance.  ReLu was used to enable a non-linear relationship.

![image](https://user-images.githubusercontent.com/100803302/178154501-02d8b92a-a29d-4a54-9a54-d83b992d2752.png)

Were you able to achieve the target model performance?
The model accuracy was .725, short of the desired 75% mark.

![image](https://user-images.githubusercontent.com/100803302/178154526-7e6e4bc7-b1e7-4f0a-a69a-27caa8e6f4c6.png)

What steps did you take to try and increase model performance?
Three additional attempts were made to meet the mark of 75%.

Attempt 1:  The only change made was to add a third layer with 20 neurons, but the accuracy remained the same - .725

![image](https://user-images.githubusercontent.com/100803302/178154553-5bd65049-a08e-45d9-9c6f-bc68813009a7.png)
![image](https://user-images.githubusercontent.com/100803302/178154588-de0b35b1-b1bd-4d16-8194-e19351acdac9.png)

Attempt 2:  The third layer remained with 25 neurons, the neurons in the first layer were increased to 100, and the neurons in the second layer were increased to 50 neurons.  The accuracy was .727.

![image](https://user-images.githubusercontent.com/100803302/178154636-d9238dab-90fc-4505-b9d5-17dbfdffa619.png)
![image](https://user-images.githubusercontent.com/100803302/178154650-052e10a7-52fc-4f2a-bfc6-30a0ddcabd02.png)

Attempt 3:  The last change was keeping the changes made in attempt 2 in place and only change the activation function to “TANH.”  This resulted in an accuracy of .726

![image](https://user-images.githubusercontent.com/100803302/178154687-43a885e0-5133-478a-9325-b6f6f9e3c0e7.png)
![image](https://user-images.githubusercontent.com/100803302/178154704-c25086f2-8245-4517-99f8-f15935396f9b.png)

Summary:

Looking at the performance metrics from the model, the neural network was able to correctly classify each of the points in the test data 73% of the time.  This accuracy score remained consistent across each of the additional attempts to reach the minimum accuracy goal of 75%. 

Because of the important to assess model performance goals prior to creating a machine learning model, this project could have been deemed successful if the accuracy goal was revised down to 72%.  Additionally, depending on the type of data and the use case, one the following could be tried to improve the accuracy score:
•	Recreate and retrain a model using different parameters
•	Use different training/test data
•	Use a different model altogether
Use of a different model, such as the ensemble-based random forest classifier, may be worth trying as an alternative due to its structural similarity to the neural network.



