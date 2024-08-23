# Sleep and Health Data Analysis

## Introduction

### Dataset Overview:
The Sleep Health and Lifestyle Dataset comprises 400 rows and 13 columns, covering a wide range of variables related to sleep and daily habits. It includes details such as gender, age, occupation, sleep duration, quality of sleep, physical activity level, stress levels, BMI category, blood pressure, heart rate, daily steps, and the presence or absence of sleep disorders.

### Key Features of the Dataset:
Comprehensive Sleep Metrics: Explore sleep duration, quality, and factors influencing sleep patterns.
Lifestyle Factors: Analyze physical activity levels, stress levels, and BMI categories.
Cardiovascular Health: Examine blood pressure and heart rate measurements.
Sleep Disorder Analysis: Identify the occurrence of sleep disorders such as Insomnia and Sleep Apnea.

## Dataset Columns:
Person ID: An identifier for each individual.
Gender: The gender of the person (Male/Female).
Age: The age of the person in years.
Occupation: The occupation or profession of the person.
Sleep Duration (hours): The number of hours the person sleeps per day.
Quality of Sleep (scale: 1-10): A subjective rating of the quality of sleep, ranging from 1 to 10.
Physical Activity Level (minutes/day): The number of minutes the person engages in physical activity daily.
Stress Level (scale: 1-10): A subjective rating of the stress level experienced by the person, ranging from 1 to 10.
BMI Category: The BMI category of the person (e.g., Underweight, Normal, Overweight).
Blood Pressure (systolic/diastolic): The blood pressure measurement of the person, indicated as systolic pressure over diastolic pressure.
Heart Rate (bpm): The resting heart rate of the person in beats per minute.
Daily Steps: The number of steps the person takes per day.
Sleep Disorder: The presence or absence of a sleep disorder in the person (None, Insomnia, Sleep Apnea).

Details about Sleep Disorder Column:

None: The individual does not exhibit any specific sleep disorder.
Insomnia: The individual experiences difficulty falling asleep or staying asleep, leading to inadequate or poor-quality sleep.
Sleep Apnea: The individual suffers from pauses in breathing during sleep, resulting in disrupted sleep patterns and potential health risks.
Acknowledgement:

I would like to clarify that the data I am presenting is synthetic and I created it for illustrative purposes.

## Objective 
This project's primary objective is to learn from Sleep Health and Lifestyle Dataset by investigating the many elements that affect the sleep and Health of people in various demographic categories.

## Data Cleaning
- Step 1 : Checked for Null Values in Excel.
- Step 2 : Checked for Duplicate Values.
- Step 3 : Split the Excel sheet to create one with People Demographics and one with Sleep and Health Data.
- Step 4 : "Person ID" column was added to both sheets to guarantee SQL join capability.
- Step 5: Created 'Age_group' column to segregate people into distinct age groups. 

## Types of Analysis

- ### Distribution Analysis 
   This analysis aims to understand the demographic data distribution across the dataset such as gender, occupation, age and BMI distribution.

- ### Sleep and Health Analysis
   This analysis aims to understand the sleep trends of the demographics across the dataset and their corresponding influence on the health trends. 

## Questions to Answer
- ### Demographics Analysis
  1. What is the numerical distribution of the Genders?
  2. What are the distinct types of BMIs and number of people under each category?
  3. What are the distinct categories of Occupations and number of people under each category?
  4. What are the distinct age groups and number of people under each age group?  
        
Snap of the query to create Age groups :

![age group column](https://github.com/user-attachments/assets/27bd4bf6-324e-4b8a-a89b-5933d1ea9414)

        
- ### Sleep and Health Analysis
  1. How do high blood pressure and heart rate influence people with sleep duration of less than 6 hours?
  2. How does sleep duration affect heart rate?
  3. Which gender is sleeping less and has a high-stress level?
  4. What is the average sleep duration and physical activity and what are their standard deviations?
  5. What are the distinct BMI categories?
  6. Analysis of the sleep duration, quality of sleep, and gender of the 25-30 age group.
  7. Is there any relationship between sleep disorders and stress levels in the age group of 25-30?
  8. What are the distinct sleep disorder categories and the most common sleep disorder?
  9. Do stress levels and occupations influence BMI?

### Snap of query
![occupation, BMI ](https://github.com/user-attachments/assets/a29c632e-779b-47c8-84f4-0de048017676)

   10. What is the average stress level of each occupation category?
   11. What is the average sleep duration of each occupation category?
   12. Which occupation has a sleep duration greater than average yet still experiences a sleep disorder?

   13. What is the most popular occupation among the age groups?
   14. Which age group has a better daily steps count?

### Snap of query

![occupation, sleep query](https://github.com/user-attachments/assets/39c5288a-7b62-4cc2-a855-f446073d8857)

  15. What is the distribution of the occupation and the most common occupation?
  16. What is the distribution of the Gender?
  17. What are the distinct age groups and their distribution?

### Snap of Age groups and their Distribution

![age group and num_people OP](https://github.com/user-attachments/assets/7e513f70-f526-4cad-922a-1b886a05feef)

  18. What is the average physical activity level by Gender?

### Snap of Gender and Physical Activity level

![gender and avg phy act](https://github.com/user-attachments/assets/dca90527-e6ed-4158-b04e-b1efdc759f55)


        
# Insights

### [1] Most people with sleep duration less than 7 hours have blood pressure greater than 120/80.

![BP and SD OP](https://github.com/user-attachments/assets/6cf39e1e-e53e-45bc-882b-fd984d67aa69)

### [2] Most people with sleep duration less than 7 hours have Stress Level greater than 6.

![sd and sl](https://github.com/user-attachments/assets/c6d73349-f3af-416f-8721-f0c377799d24)
           
### [3] Averages and Totals

    a) Avg Sleep Duration - 7.13
    b) Avg Physical Activity Level - 59.17
    c) Total Overweight - 148
    d) Total Normal weight - 216
    e) Sleep Apnea patients - 78
    f) Insomnia patients - 77
    g) Total Men - 189
    h) Total Women - 185
    i) Age groups - 21-30 - 32
                    31-40 - 133
                    41-50 - 133
                    51-60 - 76
    j) Avg Physical activity level (MEN) - 59.20
    k) Avg Physical activity level (WOMEN) - 59.14

  
  ### [4] Average Stress level by Occupation 
  
      a) Sales Representative	8.00
      b) Scientist	            7.00
      c) Salesperson	        7.00
      d) Doctor	                6.73
      e) Software Engineer	    6.00
      f) Nurse	                5.55
      g) Lawyer	                5.06
      h) Manager	            5.00
      i) Accountant	            4.59
      j) Teacher	            4.53
      k) Engineer	            3.89

  ### [5] Average Sleep Duration by Occupation
      a) Sales Representative	5.9
      b) Scientist	            6
      c) Salesperson	        6.4
      d) Teacher	            6.69
      e) Software Engineer	    6.75
      f) Manager	            6.9
      g) Doctor	                6.97
      h) Nurse	                7.06
      i) Accountant	            7.11
      j) Lawyer	                7.41
      k) Engineer	            7.99

 ### [6] Compared to women, more men between the ages of 25 and 30 have sleep durations of less than 7.

 ### [7] Compared to men, more women between the ages 25 and 55 have a sleep disorder.

 ### [8] Those in the overweight BMI category who work as nurses have higher levels of stress than the average for their occupational group, followed by Salesperson occuaption.

 ![avg stress occupation](https://github.com/user-attachments/assets/9959a676-8292-429c-b60f-7f9470316429)

### [9] Most people with sleep disorders are nurses. Most people with Sleep Apnea are also nurses.

![occupation and sleep disorder](https://github.com/user-attachments/assets/cca2f383-94e1-471e-979e-f88efd686e00)

### [10] Most people with no sleep disorders are Doctors, followed by Engineers.

![occupation and no sleep dis](https://github.com/user-attachments/assets/1266f165-fc0e-49ae-bc90-5f5c4b4e1abf)

### [11] Majority of the people belong to the age group 31-50.

### [12] Individuals between the ages of 21 and 30 have the highest average stress level.

![age group and avg stress](https://github.com/user-attachments/assets/c08520e6-e105-4df9-a26c-981c82b54b5f)

### [13] The most popular occupation among the age groups 21-30 and 31-40 is Doctor.

![age and pop occuoation](https://github.com/user-attachments/assets/dabca882-7572-463f-ac66-5d6cfa57f0b3)
 
### [14] People of the age group 41-50 have the most avg. daily steps count and people of the age group 51-60 have the lowest avg. daily steps count.

![age groups and steps](https://github.com/user-attachments/assets/4c3dc295-5b46-4441-a30a-7c03586fdab0)

