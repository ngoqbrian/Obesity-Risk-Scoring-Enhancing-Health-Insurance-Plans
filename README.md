Introduction

Data has a large potential to positively impact us now more than ever, which is why I chose to analyze a dataset that estimated obesity levels based on the eating habits and physical condition of people from Mexico, Peru, and Colombia. I was interested in the relationship between body fat levels and lifestyle habits, as the findings can be applicable to the health and wellbeing of many, if not most, of us. It is especially relevant because BMI has been on the news a lot recently due to the fact that those with a high BMI are eligible to get the COVID-19 vaccine earlier, as obese individuals are three times more likely to be hospitalized from the virus. I used a dataset from UC Irvine’s Machine Learning Repository, which included the data of 2111 individuals ages 14 to 61.

The dataset had 17 attributes, many of which have acronyms for ease of coding, so I will give briefly describe all of the attributes:

    Gender: female or male
    Age: numeric
    Height: numeric, in meters
    Weight: numeric, in kilograms
    family_history (family history of obesity): yes or no
    FCHCF (frequent consumption of high caloric food): yes or no
    FCV (frequency of consumption of vegetables: 1, 2, or 3; 1 = never, 2 = sometimes, 3 = always
    NMM (number of main meals): 1, 2, 3 or 4
    CFBM (consumption of food between meals): 1, 2, 3, or 4; 1=no, 2=sometimes, 3=frequently, 4=always
    Smoke: yes or no
    CW (consumption of water): 1, 2, or 3; 1 = less than a liter, 2 = 1–2 liters, 3 = more than 2 liters
    CCM (calorie consumption monitoring): yes or no
    PAF (physical activity frequency per week): 0, 1, 2, or 3; 0 = none, 1 = 1 to 2 days, 2= 2 to 4 days, 3 = 4 to 5 days
    TUT (time using technology devices a day): 0, 1, or 2; 0 = 0–2 hours, 1 = 3–5 hours, 2 = more than 5 hours
    CA (consumption of alcohol): 1, 2, 3, or 4; 1= never, 2 = sometimes, 3 = frequently, 4 = always
    Transportation: automobile, motorbike, bike, public transportation, or walking
    Obesity**: insufficient weight, normal weight, level I overweight, level II overweight, type I obesity, type 2 obesity, type 3 obesity; these categories are listed from lowest to highest body fat

**Note: I will refer to these categories as “weight classifications” and “body fat levels”, but they are not determined solely by one’s weight or body fat level.

Given these attributes, I approached this project with the goal of trying to find the answers to the following questions:

    As the makeup of respondents is important to the conclusions derived from this dataset, what kinds of characteristics do the people in this dataset have?
    Can BMI be used as a quantitative substitute for the qualitative weight classification category?
    Which eating habit and physical condition variables are most related to obesity levels? This question has many subquestions related to individual variables and groups of variables.
