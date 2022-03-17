# Neural_Network_Charity_Analysis

## Overview
The purpose of this project is to use my knowledge of machine learning and neural networks, I will use the features in the provided dataset to help Beks create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

## Results
- During data preporcessing, I removed columns EIN and NAME from the input data.
- I will use IS_SUCCESSFUL column data to consider target for my modeling. And columns APPLICATION_TYPE, APPLICATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS and ASK_AMT are my feature variable for my modeling.
![Capturefirst attempt](https://user-images.githubusercontent.com/92561493/158744435-8575d7be-64c0-43b1-80cd-20f93e3cb5a9.PNG)
- In my first attempt, I dropped three more data columns ['AFFILIATION_Other','USE_CASE_Other','APPLICATION_TYPE_Other']). And I used 2 layers, 16 neurons for the first and 10 neurons for the second layers. The result is 72.57% which is lower than the target 75%.
![Capturefirst 2nd attempt](https://user-images.githubusercontent.com/92561493/158744436-1ef3384c-530c-4a2c-8bb5-e8108f9328e6.PNG)

- In my second attempt, I added one more layer. And increased neurons for first layer to 30; second layer to 25 and third layer is 10. Also I used activation "Linear" for first, second, third layers. And "sigmoid" for output layer, The result is 71.87% which is lower than target 75%,

![Capturefirst 3rd attempt](https://user-images.githubusercontent.com/92561493/158744437-6d566da2-8249-440e-93e1-b60709d93963.PNG)
-In my third attempt, I added one more layer. There are total 4 layers with 90,70,50 and 40 neurons repectively. I used "relu" activation for first 3 layers and "sigmoid" for outer layer. The result is 72.65% which is lower than 75%.

## Summary
Throughout my 3 attempts, my hight performance is 72.65% which is lower than target 75%. Threre are more ways to imporve the performance such as removing more noisy variables from features, adding more layers or neurons or using other activations in layers etc. Since our model is not outperforming with target result, we should try to use other supervised manchine learning model such as Random Forest model.
