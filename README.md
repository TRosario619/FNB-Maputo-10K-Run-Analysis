# Maputo FNB 10 KM Run Results Analysis

## Overview

This project explores the results dataset of a running event I participated, with the aim of answering specific questions through data analysis.

## Questions Explored

1. **Variation in race completion positions**
2. **Fastest finish time by Class**
3. **Countries participation**
   - Top 3 finishes per country
4. **Top finishes by Class and Gender**
5. **Percentile analysis**
   - Overall and per category
6. **Average pace of Top 10 racers in My Class**

## Steps

### 1. Data Overview
The dataset was extracted from PeakTiming page for the [FNB Maputo 10K Race](https://live.ultimate.dk/desktop/front/index.php?eventid=5987), by copying to a csv file. 
Data Dictionary:
    - Rank: Indicates the overall rank of the race
    - Race No: Runner Id number
    - Name: The Name of the runner
    - Nation: The Nation of the Runner
    - Categoria: The Class of the Runner
    - Category: It's a concatenation of Gender and age group 
    - Time: Total race time of the runner

The analysis is focused on 4 key columns, Namely: 'Rank', 'Categoria', 'Category' and 'Time'. 

### 2. Exploratory Data Analysis (EDA)

- When loading the data, I firstly checked for for null data, duplicates, removed columns deemed unnecessary and converted column data types where appropriate for analysis. I renamed two columns with the same name (in different languages: changed Categoria to Class) in the dataset that could create confusion and aligned the classes of runners reducing them to 3. Also feature engineered data coming from category  and Time, such as gender, age group, ranks per class and category to assist in answering project questions.
  
### 3. Findings

- The initial surge of race finishes occurs around the first hour of the race, followed by a second peak slightly before the second hour. Interestingly, the first peak is predominantly comprised of male participants, while the second peak is mostly female.

- Notably, the professional class (**FEDERADOS**) achieved faster finishes compared to other classes. On average, they completed the race a minute earlier than the popular class (**POPULARES**) and three minutes earlier than the veterans class (**VETERANOS**).

- A total of 24 countries participated in the event, with Mozambique leading with 2170 participants, followed by Swaziland, Portugal, and South Africa with 20, 12, and 10 participants, respectively.

- South Africa, Namibia, and New Zealand were the only countries represented on the podiums for each class and gender, in addition to Mozambique.

- I achieved a ranking in the top 17% overall, the top 16% in my class (**POPULARES**), and the top 27% in my category (**M 20-39**).

- To break into the top 10 of my class and category, I would need to improve my average pace per kilometer from 5 minutes and 55 seconds to below 3 minutes and 45 seconds.

### 4. Conclusion

- The order of class performance did not surprise me, but I was not expecting the gap between the professional class and the other classes to be close to 1-2 minutes. This suggests that you don't need to be a professional to be a great runner.
- It was gratifying to discover that Mozambican people enjoy participating in events that promote health and well-being.
- I am determined to keep training and improving to reach the top tier. Hopefully, next year will bring even better results!
- This project provided a valuable opportunity to explore pandasql, a library for querying pandas dataframes with SQL. It was both interesting and straightforward to use, particularly for certain types of questions.

## Dependencies

- This project was the done in and environment with the following tools/libraries:
    - python: 3.9.12
    - pandas
    - pandasql
    - matplotlib
    - seaborn

Thank you for looking into the project. If you have suggestions to improve the analysis, identify patterns, or enhance visualizations, please share your thoughts. Looking forward to diverse perspectives that contributors bring to the table.