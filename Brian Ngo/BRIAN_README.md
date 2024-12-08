



















# Brian's Analysis:




## Exploratory Data Analysis:

### The Correlation of Height and Weight with Obesity Classification

![Figure 1](https://raw.githubusercontent.com/ngoqbrian/Obesity-Risk-Scoring-Enhancing-Health-Insurance-Plans/Team-Project-1/Brian%20Ngo/images/figure1.png)






![Figure 2](https://raw.githubusercontent.com/ngoqbrian/Obesity-Risk-Scoring-Enhancing-Health-Insurance-Plans/Team-Project-1/Brian%20Ngo/images/figure2.png)




### Heatmap

![Figure 3](https://raw.githubusercontent.com/ngoqbrian/Obesity-Risk-Scoring-Enhancing-Health-Insurance-Plans/Team-Project-1/Brian%20Ngo/images/figure3.png)








### Classifications:
Which attributes related to eating habits and physical conditions most significantly predict obesity levels, as categorized by the NObesity classification system?

#### Linear Regression Model for BMI

![Figure 4](https://raw.githubusercontent.com/ngoqbrian/Obesity-Risk-Scoring-Enhancing-Health-Insurance-Plans/Team-Project-1/Brian%20Ngo/images/figure4.png)



For our linear regression model, we identified several key factors that influenced BMI.

-Weight  
    Managing weight through

-Family History of Overweight


-Dietary Habits





Feature Coefficients:
Height                                   -32.632894
Weight                                     0.331337
CAEC_encoded                               0.224688
FCVC                                       0.234303
FAVC_encoded                               0.234859
family_history_with_overweight_encoded     0.650761
FAF                                       -0.047631
SCC_encoded                               -0.400499
dtype: float64
intercept: 54.88626762904084


Weight is a significant actionable predictor affecting BMI

Family History

Dietary Habits

Phyiscal Activity

Behavioural Awareness - Monitoring


#### Random Forest Analysis for Obesity Classification

![Figure 5](https://raw.githubusercontent.com/ngoqbrian/Obesity-Risk-Scoring-Enhancing-Health-Insurance-Plans/Team-Project-1/Brian%20Ngo/images/figure5.png)


Accuracy: {0.9353312302839116}
Classification Report:
               precision    recall  f1-score   support

           0       0.94      0.95      0.95        86
           1       0.80      0.90      0.85        93
           2       0.98      0.94      0.96       102
           3       0.97      0.99      0.98        88
           4       1.00      0.99      0.99        98
           5       0.90      0.84      0.87        88
           6       0.97      0.92      0.95        79

    accuracy                           0.94       634
   macro avg       0.94      0.93      0.94       634
weighted avg       0.94      0.94      0.94       634











