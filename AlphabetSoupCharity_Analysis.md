# AlphabetSoupCharity_Analysis

## Overview
Using a CSV from Alphabet Soup containing more than 34,000 organizations that have received funding from Alphabet Soup over the years, a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup will be created. 

## Results
### Data Preprocessing:

  * What variable(s) are considered the target(s) of your model?
    * The column labeled 'IS_SUCCESSFUL' is considered the target for this model.

  * What variable(s) are considered the features of your model?
    * Variables that are features include: APPLICATION_TYPE, AFFILICATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS and ASK_AMT. 

  * What variable(s) are neither targets nor features and should be removed from the input data?
    * EIN and NAME are neither targets nor features and are dropped from the dataframe. 

### Compiling, Training and Evaluating the Model

 * How many neurons, layers and activation functions did you select for your neural network model and why? Were you able to achieve the target model performance? What steps did you take in your attempts to increase model performance?

  * First Attempt - Using only 2 layers, the target model did performance did not reach 75% accuracy (63%)
  ![image](https://github.com/marthagriggs9/deep-learning-challenge/assets/115905663/75f62f77-0600-43f6-90ce-0fcae4cbe185)
  
  ![image](https://github.com/marthagriggs9/deep-learning-challenge/assets/115905663/4d219ccf-78bc-4206-9177-1b463c1f1374)


  * Second Attempt - Added a 3rd hidden layer and the model performance accuracy went down to 61%. I switched the activation function from 'relu' to 'tanh'. 
  ![image](https://github.com/marthagriggs9/deep-learning-challenge/assets/115905663/adc17a7e-9867-48d0-b40c-beff5a909484)
  
  ![image](https://github.com/marthagriggs9/deep-learning-challenge/assets/115905663/6e07931f-b523-4faf-a77f-ee14df7662b5)

  * Third Attempt - Again, I used 3 layers, but increased the first and third layers neurons by 10. I again used the 'tanh' activation function. This model was much closer to the target model performance of 75%, but it was not able to reach the 75% accuracy that was desired. 

![image](https://github.com/marthagriggs9/deep-learning-challenge/assets/115905663/51fe1ee6-b96a-4876-aec0-ca34289f7d95)

![image](https://github.com/marthagriggs9/deep-learning-challenge/assets/115905663/b8d224ee-4001-4f49-92c5-cc7fcb6df543)

### Summary
In the three attempts, the model failed to reach the target model performance of 75% accuracy. A recommendation for reaching that accuracy or higher would be to add or gather more data to add to the dataset to make it larger. Using a different classification model (multi-class or multi-label) could also lead to better predicting on whether applicants will be successful if funded by Alphabet Soup. 
