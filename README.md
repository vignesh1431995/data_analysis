## Problem Statement
Every year, American high school students take SATs, which are standardized tests intended to measure literacy, numeracy, and writing skills. There are three sections - reading, math, and writing, each with a maximum score of 800 points. 
These tests are extremely important for students and colleges, as they play a pivotal role in the admissions process.
Analyzing the performance of schools is important for a variety of stakeholders, including policy and education professionals, researchers, government, and even parents considering which school their children should attend.
You have been provided with a dataset called schools.csv, which is previewed below.
You have been tasked with answering three key questions about New York City (NYC) public school SAT performance.

## To Find : 
1. Which NYC schools have the best math results?
2. What are the top 10 performing schools based on combined SAT scores?
3. Which single borough has the single largest standard deviation in the combined SAT score?

## Given :
1. The best math results are at least 80% of the *maximum possible score of 800* for math.

## Steps Followed
1. Import The csv file - schools.csv into Data Frame - schools
2. We Explored the columns present in the imported csv file.
3. We create a new Data Frame 'best_math_schools' which holds the school_name and average_math score columns with average math score >=640 (80% of 800) and sort the values in descending order of average_math column. (Answer #1)
4. We create a new columns in 'total_SAT' in Data Frame 'schools' which is a sum of average_math, average_reading and average_writing columns for each row.
5. We create a new Data Frame 'top_10_schools' by selecting the top 10 rows based on 'total_SAT' column from data frame 'schools'. (Answer #2)
6. We calculate the Average, Median and Standard Deviation of 'total_SAT' column for schools by 'borough' column and store in Data Frame 'schools_std_dev'.
7. We pick the school with largest standard deviation from the data frame 'schools_std_dev' (Answers #3)
