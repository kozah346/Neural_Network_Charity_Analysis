# Neural_Network_Charity_Analysis
## Overview of the analysis
* The following analysis is done for a foundation to predict where to make investments using machine learning and neural networks. Using features in the provided dataset, a binary classifier is created that is capable of predicting whether applicants will be successful if funded by the foundation, Alphabet Soup. 
* The analysis is conducted using a dataset of a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. The following columns capture metadata about each organization  as follows: 
  1. EIN and NAME—Identification columns
  2. APPLICATION_TYPE—Alphabet Soup application type
  3. AFFILIATION—Affiliated sector of industry
  4. CLASSIFICATION—Government organization classification
  5. USE_CASE—Use case for funding
  6. ORGANIZATION—Organization type
  7. STATUS—Active status
  8. INCOME_AMT—Income classification
  9. SPECIAL_CONSIDERATIONS—Special consideration for application
  10. ASK_AMT—Funding amount requested
  11. IS_SUCCESSFUL—Was the money used effectively


## Results
### Data Preprocessing
* The variable **IS_SUCCESSFUL** is considered the target for the model as shown below: <img width="1186" alt="Targets" src="https://user-images.githubusercontent.com/101376325/182066103-4034ec53-a6cb-41f2-998f-1efc4a12f66f.png">

* The variables shown in the image below are features for the model: <img width="1185" alt="Model Features" src="https://user-images.githubusercontent.com/101376325/182066298-df9e5633-ed87-4369-90bf-bba4d6c85d61.png">

* The two variables **EIN** and **NAME** are neither targets nor features and are therefore dropped as shown below: <img width="1198" alt="Non_Beneficial" src="https://user-images.githubusercontent.com/101376325/182066574-32cd9a42-e58e-4d5d-a8b2-aecf79fccdde.png">

### Compiling, Training, and Evaluating the Model

* The images below shows steps taken to improve the model perfomance:
  <img width="926" alt="Try1" src="https://user-images.githubusercontent.com/101376325/182067014-6e071d26-be37-4303-9813-55a45f7edb04.png">

  <img width="1063" alt="Try2" src="https://user-images.githubusercontent.com/101376325/182067042-fdd9da52-bb0f-443c-882a-58a3cdcc152a.png">

  <img width="1045" alt="Try 3" src="https://user-images.githubusercontent.com/101376325/182067092-40c01455-25ed-49a4-a9ea-da0654469b4d.png">

* In all the images, the number of layers was increased from 2 to 3. 
* In the second image, the number of hidden nodes was increased to 100 for each layer.
* In the third image, the activation function in the hidden layers was changed from **relu** to **linear**. 
* Despite all the steps mentioned above, the target model perfomance of 75% was not achieved.

## Summary
In conclusion, the model failed to achieve the required target model perfomance hence will require a different approach which can be a RandomForestClassifier. It could work in the sense that many weak decision trees are combined into strong decision trees hence a good model is developed. 
  
   


