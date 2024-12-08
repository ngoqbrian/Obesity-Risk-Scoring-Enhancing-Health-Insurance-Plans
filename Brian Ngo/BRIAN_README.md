# **Brian Ngo's Analysis**:

## Project Overview:  
This project aims to classifiy obesity levels using a data-drive approach to provide actionable insights for health insurers. By creating classification models that identify key predictors of obesity, health insurers will be able to create personalized and targeted health insurance plans based on an individual's health, lifesytle, and demographic attributes.

### Objectives:
-Build a predictive model for obesity classification using health and lifestyle features  
-Identify critical factors influencing obesity to inform personalized insurance plans  
-Enable insurers to create risk-adjusted, targeted plans that promote healthier behaviors and mitigate associated health risks  

**[View Brian's Jupyter Notebook for Obesity Risk Scoring Data Analysis](https://github.com/ngoqbrian/Obesity-Risk-Scoring-Enhancing-Health-Insurance-Plans/blob/Team-Project-1/Brian%20Ngo/src/Obesity_Brian.ipynb)**

## **Exploratory Data Analysis**:

### The Correlation of Height and Weight with Obesity Classification

![Figure 1](https://raw.githubusercontent.com/ngoqbrian/Obesity-Risk-Scoring-Enhancing-Health-Insurance-Plans/Team-Project-1/Brian%20Ngo/images/figure1.png)

### Family History of Overweight and Obesity Classification

![Figure 2](https://raw.githubusercontent.com/ngoqbrian/Obesity-Risk-Scoring-Enhancing-Health-Insurance-Plans/Team-Project-1/Brian%20Ngo/images/figure2.png)

### Heatmap

![Figure 3](https://raw.githubusercontent.com/ngoqbrian/Obesity-Risk-Scoring-Enhancing-Health-Insurance-Plans/Team-Project-1/Brian%20Ngo/images/figure3.png)

## **Obesity Classification Models**:

### Linear Regression Model for BMI

![Figure 4](https://raw.githubusercontent.com/ngoqbrian/Obesity-Risk-Scoring-Enhancing-Health-Insurance-Plans/Team-Project-1/Brian%20Ngo/images/figure4.png)

Our linear regression model identified several key factors that influenced BMI:  
-Weight  
-Family History of Overweight  
-Dietary Habits (FCVC, FAVC)  
-Calorie Consumption Monitoring (SCC_encoded) 

#### **Feature Coefficients**:
- Height: -32.63
- Weight: 0.33
- CAEC (Eating Between Meals): 0.22
- FCVC (Frequency of Vegetable Consumption): 0.23
- FAVC (Frequent High-Calorie Food Consumption): 0.23
- Family History of Overweight: 0.65
- FAF (Frequency of Physical Activity): -0.05
- SCC (Calorie Monitoring): -0.40  
Intercept: 54.89

**Model Performance**:  
**Mean Squared Error (MSE)**: **0.63**  
**R-squared (R^2)**: **0.99**

### Random Forest Analysis for Obesity Classification

![Figure 5](https://raw.githubusercontent.com/ngoqbrian/Obesity-Risk-Scoring-Enhancing-Health-Insurance-Plans/Team-Project-1/Brian%20Ngo/images/figure5.png)

Weight is the most significant predictor for obesity classificaiton, which aligns with its direct influence on Body Mass Index (BMI).  
Frequency of Vegetable Consumption (FCVC), Phyiscal Activity Frequency (FAF) and Time Using Techonology (TUE) are important lifestyle predictors in classifying obesity.  

**Model Performance**:  
**Accuracy**: **93.53%**  
**F1-Score** (Macro Average): **0.94**  
**Precision** (Macro Average): **0.94**  
**Recall** (Macro Average): **0.93**  

| **Class**                | **Precision** | **Recall** | **F1-Score** | **Support** |
|---------------------------|---------------|------------|--------------|-------------|
| Insufficient Weight (0)   | 0.94          | 0.95       | 0.95         | 86          |
| Normal Weight (1)         | 0.80          | 0.90       | 0.85         | 93          |
| Overweight Level I (2)    | 0.98          | 0.94       | 0.96         | 102         |
| Overweight Level II (3)   | 0.97          | 0.99       | 0.98         | 88          |
| Obesity Type I (4)        | 1.00          | 0.99       | 0.99         | 98          |
| Obesity Type II (5)       | 0.90          | 0.84       | 0.87         | 88          |
| Obesity Type III (6)      | 0.97          | 0.92       | 0.95         | 79          |
| **Accuracy**              |               |            | **0.94**     | 634         |
| **Macro Average**         | 0.94          | 0.93       | 0.94         |             |
| **Weighted Average**      | 0.94          | 0.94       | 0.94         |             |

## **Conclusion**:
This project highlights the value of obesity risk socring through predictive models (Linear Regression and Random Forest). By accurately classifying obesity levels and quantifying the influence of key predictors, insurers can use these models to inform strategic data-driven decision making. These models provide an opportunity to improve obesity related risk predictions, which can help predict healthcare costs more accurately based on obesity classifications. They also provide an opporunity to create personlized plans for health policyholders and cost savings for insurers by implementing early interventions that can reduce claims related to obesity-related conditions

Insurers will be able to create personalized plans through several methods:
1. Premium adjustments
2. Preventive Health Benefits
3. Behavioural Incentives

By adjusting premiums to reflect an individual and provide a more personalized approach, health policyholders will be more incentivized and informed in seeking the best plan available. Insurers can offer preventive health benefits through weight management programs, gym membership discounts, and nutrition counselling as a way to decrease obesity-related health conditions (diabetes, hypertension, and hearth disease). These benefits encourage policyholders to adopt healthier lifestyles, thereby reducing long-term healthcare costs for both insurers and individuals. Behavioural incentives such as rewards for increasing physical activity or premium reductions for consistent improvement in obesity level can improve customer satisfaction and incentivize healthier behaviours.

The data-driven insights from these models demonstrate how leveraging obesity risk scoring can allow insurers to design targeted health plans, promote preventive care, and encourage healthier lifestyles, ultimately benefiting both policyholders and the healthcare system.

## **Video Submission Link**:  
### Brian's Video:  
- [Download from GitHub](https://github.com/ngoqbrian/Obesity-Risk-Scoring-Enhancing-Health-Insurance-Plans/blob/Team-Project-1/Brian%20Ngo/images/Brian_Video_Sub.mp4)  
- [Stream on Google Drive](https://drive.google.com/file/d/1dSS0fj6amqV6dqQpkqlKSV__3FkLLORW/view?usp=drive_link)



