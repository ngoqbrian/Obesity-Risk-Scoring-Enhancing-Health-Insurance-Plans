# **Enhanced Health Insurance Plans Based on Obesity Risk-Scoring**  
## **Project Overview**  
Welcome to the "Enhanced Health Insurance Plans Based on Obesity Risk-Scoring"! The project focuses on analyzing and optimizing health insurance plans based on obesity risk scoring.

What is Obesity?

Having a body weight that is higher than what is considered healthy for a given height is described as obesity. There are many methods of measuring this, some of which are expensive and time consuming. BMI, which is inexpensive and easy to calculate, is typically used as a proxy. Health officials recommend that individual health assessments should take into consideration other factors as well. Research has demonstrated that a high BMI is strongly correlated with negative health consequences, although the BMI values vary among various ethnic groups.

BMI is characterized by a greater weight to hight ratio. BMI is a person’s weight in kilograms divided by their height in meters squared. For measurements in pounds and inches, BMI is calculated using the following formula: BMI = 703 x weight (pounds) / height (inches) squared. 

Defining Obesity Among Children and Teens

Because kids are still growing, obesity is measured differently among children than adults. Instead of a simple BMI measurement, a child’s BMI is compared to others of the same age and sex.
According to the Centers for Disease Control and Prevention (CDC), child obesity is defined as a BMI that is at or above the 95th percentile for children and teens of the same age and sex. Overweight is defined as a BMI that is at or above the 85th percentile and below the 95th percentile for children and teens of the same age and sex.

Why is BMI age- and sex-specific for children and teens?

A child’s weight status is determined using an age- and sex-specific percentile for BMI, which is different from BMI categories used for adults. Because children’s body fat levels change over the course of childhood and vary between boys and girls, their BMI levels are expressed relative to other children of the same age and sex.

**Team Members **   
Anca Kurian  
[Brian Ngo](#brian-ngos-analysis)  
Mariam Ibrahim  
MD Razaul Karim  


Data Introduction

Data has a large potential to positively impact us now more than ever, which is why I chose to analyze a dataset that estimated obesity levels based on the eating habits and physical condition of people from Mexico, Peru, and Colombia. I was interested in the relationship between body fat levels and lifestyle habits, as the findings can be applicable to the health and wellbeing of many, if not most, of us. It is especially relevant because BMI has been on the news a lot recently due to the fact that those with a high BMI are eligible to get the COVID-19 vaccine earlier, as obese individuals are three times more likely to be hospitalized from the virus. I used a dataset from UC Irvine’s Machine Learning Repository, which included the data of 2111 individuals ages 14 to 61.

The dataset had 17 attributes, many of which have acronyms for ease of coding, so I will  briefly describe all of the attributes:

    Gender: female or male
    Age: numeric
    Height: numeric, in meters
    Weight: numeric, in kilograms
    family_history (family history of obesity): yes or no
    FCHCF (frequent consumption of high caloric food): yes or no
    FCV (frequency of consumption of vegetables: 1, 2, or 3; 1 = never, 2 = sometimes, 3 = always)
    NMM (number of main meals): 1, 2, 3 or 4
    CFBM (consumption of food between meals): 1, 2, 3, or 4; 1 = no, 2 = sometimes, 3 = frequently, 4 = always
    Smoke: yes or no
    CW (consumption of water): 1, 2, or 3; 1 = less than a liter, 2 = 1–2 liters, 3 = more than 2 liters
    CCM (calorie consumption monitoring): yes or no
    PAF (physical activity frequency per week): 0, 1, 2, or 3; 0 = none, 1 = 1 to 2 days, 2 = 2 to 4 days, 3 = 4 to 5 days
    TUT (time using technology devices a day): 0, 1, or 2; 0 = 0–2 hours, 1 = 3–5 hours, 2 = more than 5 hours
    CA (consumption of alcohol): 1, 2, 3, or 4; 1 = never, 2 = sometimes, 3 = frequently, 4 = always
    Transportation: automobile, motorbike, bike, public transportation, or walking
    Obesity**: insufficient weight, normal weight, level I overweight, level II overweight, type I obesity, type 2 obesity, type 3 obesity; these categories are listed from lowest to highest body fat

Rules of Engagement

    Transparent and clear communication among team members.
    Collaboration and teamwork.
    Respect and professionalism in sharing different viewpoints.
    Leveraging each team member's expertise for effective project contributions.
    Conducting regular team meetings and summarizing key discussion points.
    Open idea-sharing.
    Providing support for team members facing difficulties.
    Commitment to continuous improvement.

Context & Problem
Obesity and related health conditions, such as diabetes, cardiovascular diseases, and hypertension, are major contributors to the rising cost of medical insurance. Insurance companies face higher claims from individuals with these conditions, leading to an overall increase in premiums. By analyzing lifestyle habits, we can predict obesity levels and identify high-risk individuals before they develop severe medical conditions, thus reducing health insurance costs in the long term.

The provided dataset contains information on individuals' demographics, eating habits, physical activity, and obesity levels. Predictive analytics can be used to forecast an individual’s obesity risk based on their lifestyle habits. With this information, insurance companies can implement preventative measures, personalized health plans, and adjust insurance premiums based on predicted health outcomes

Key Features in the Dataset
The dataset includes lifestyle factors that influence health:

Demographics: Gender, Age, Height, Weight
Dietary habits: Family history with obesity, frequent consumption of high-calorie foods (FAVC), daily meals (NCP), consumption of alcohol (CALC)
Physical activity: Physical activity frequency (FAF), transportation mode (MTRANS)
Health-related factors: Smoking (SMOKE), hydration (CH2O), sedentary time (TUE)

Predictive Analytics Workflow
Problem Definition:
We aim to predict the obesity level of individuals (target variable: NObeyesdad) using various features related to lifestyle habits. By predicting obesity early, we can intervene with tailored health programs or adjust insurance premiums.

![Obesity ML Flow ](https://github.com/user-attachments/assets/00db4eaf-435d-475d-857c-d4398093841f)

Data Preprocessing:
1. Understanding the Data
The dataset includes key features like Gender, Age, Height, Weight, BMI, Smoking habits, Family history of overweight, and lifestyle factors (e.g., exercise frequency, water intake, etc.), which can be crucial in predicting obesity and its correlation with medical costs.

2. Exploration & Discovery
Exploratory data analysis (EDA) is the starting point to uncover trends:

![image](https://github.com/user-attachments/assets/d62ac2d9-d670-446a-88a1-b1c3b4c097cc)


Correlation Analysis: Examine potential correlation relationships between lifestyle habits (like smoking, alcohol consumption, exercise) and obesity.
Visualization: Use scatter plots, histograms, and heatmaps to see the distribution of obesity across gender, age, and lifestyle choices.

3. Business Case
The analysis will provide insights for:


![image](https://github.com/user-attachments/assets/ec5d2627-95b8-416e-9a06-b4a9ce9d0477)


Insurers: By identifying lifestyle risks like smoking or lack of physical activity, insurers can design tailored premiums based on risk levels.
Insurance Buyers: Buyers adopt healthier lifestyle habits to reduce insurance costs by avoiding risk categories such as smoking or high BMI.

4. Technical Solution
To address the business case, the following techniques have been employed:

![image](https://github.com/user-attachments/assets/8a4698c7-9a1c-4b4e-8fad-d70d233cdda5)

a. KNN Classification
Goal: Predict obesity class or risk levels based on features like age, BMI, and lifestyle habits.
Application: Classify whether an individual is at high or low risk of obesity-related conditions, which can directly impact their insurance premiums.
b. Regression Models
Goal: Predict BMI or medical costs based on factors such as age, weight, and exercise frequency.
Application: Use linear regression or other models to understand how different habits influence BMI and, indirectly, healthcare costs.
c. Clustering

![image](https://github.com/user-attachments/assets/98ab5d83-3815-418a-96bf-bf5623753adc)

Goal: Group individuals into clusters based on similar lifestyle patterns (e.g., smokers vs. non-smokers, active vs. sedentary).
Application: This segmentation can allow insurers to identify low- and high-risk groups for customized policy offerings.

Interactive Dashboard 

![Obesity_Dashboard_snapshot](https://github.com/user-attachments/assets/e97a9a08-0942-482b-886c-d7b56b6c6d92)

Dashboard storytelling 
Power BI dashboard tailored to an insurance business using the obesity dataset, focusing on visualizations that highlight risk factors, cost implications, and target groups for optimized insurance strategies. Here's a step-by-step approach for designing an effective dashboard.

1. Prepare Data in Power BI
Data Preparation: Import the obesity dataset into Power BI and clean it by checking for missing or inconsistent data.
Create Calculated Columns: For example, you may want to categorize individuals into age groups or label BMI ranges as “Normal,” “Overweight,” “Obese,” etc., depending on BMI values.
Data Model: Establish relationships between tables if using other datasets (e.g., healthcare cost data, lifestyle information).
2. Design Dashboard Elements
A. High-Risk Group Identification
Bar Chart: Display the count of individuals in each obesity category (e.g., Normal, Overweight, Obese).
Stacked Bar Chart or Matrix: Show high-risk lifestyle factors such as smoking and low physical activity by obesity category to visually separate risk levels.
B. Average Healthcare Costs by Obesity Level
Line and Clustered Column Chart: Compare average healthcare costs across obesity levels, overlayed with age groups, to show which groups drive higher costs.
Gauge Chart: Represent average healthcare cost, with a dynamic gauge that updates based on filters like obesity level or lifestyle factors.
C. Age Group and BMI Analysis
Heatmap or Matrix Table: Display average BMI by age group to quickly spot which demographics have the highest obesity levels.
Clustered Column Chart: Compare BMI and healthcare costs across age groups, helping to pinpoint age ranges where intervention might be needed most.
D. Physical Activity and Cost Savings Analysis
Scatter Plot: Plot physical activity levels against healthcare costs for each obesity category. This helps identify cost-saving opportunities by promoting physical activity.
Card Visuals: Show metrics like “Average Cost for Low Physical Activity,” “Average Cost for High Physical Activity,” or “Cost Savings from Increased Activity.”
E. Risk Factor Comparison by Lifestyle Choices
Stacked Column Chart: Show a breakdown of obesity levels for different smoking statuses and alcohol consumption levels to assess the impact of lifestyle choices.
Donut Chart: Use a donut chart to illustrate the percentage of high-risk lifestyle choices (e.g., smoking, alcohol consumption) within obese and overweight categories.
KPI Cards: Display metrics such as “Suggested Premium Adjustment” based on high-risk behaviors or healthcare cost averages.
Table with Conditional Formatting: Display a table of individuals or customer segments with high obesity levels and costs above average, with conditional formatting to highlight the most severe cases.
3. Adding Interactivity and Filters
Filters: Include slicers for Age Group, Obesity Level, Smoking Status, Alcohol Consumption, and Physical Activity.




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

