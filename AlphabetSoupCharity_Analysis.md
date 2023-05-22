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
