# Pandas_Challenge

In this assignment, you’ll create and manipulate Pandas DataFrames to analyze school and standardized test data.

## Background
You are the new Chief Data Scientist for your city's school district. In this capacity, 
you'll be helping the school board and mayor make strategic decisions regarding future school budgets and priorities.

As a first task, you've been asked to analyze the district-wide standardized test results. 
You'll be given access to every student's math and reading scores, as well as various information on the schools they attend. 
Your task is to aggregate the data to showcase obvious trends in school performance.

## District Summary
Perform the necessary calculations and then create a high-level snapshot of the district's key metrics in a DataFrame.
Include the following:
Total number of unique schools
Total students
Total budget
Average math score
Average reading score
% passing math (the percentage of students who passed math)
% passing reading (the percentage of students who passed reading)
% overall passing (the percentage of students who passed math AND reading)

##School Summary
Perform the necessary calculations and then create a DataFrame that summarizes key metrics about each school.
Include the following:

School name
School type
Total students
Total school budget
Per student budget
Average math score
Average reading score
% passing math (the percentage of students who passed math)
% passing reading (the percentage of students who passed reading)
% overall passing (the percentage of students who passed math AND reading)

##Highest-Performing Schools (by % Overall Passing)

Sort the schools by % Overall Passing in descending order and display the top 5 rows.
Save the results in a DataFrame called "top_schools".
Lowest-Performing Schools (by % Overall Passing)
Sort the schools by % Overall Passing in ascending order and display the top 5 rows.
Save the results in a DataFrame called "bottom_schools".

## Math Scores by Grade
Perform the necessary calculations to create a DataFrame that lists the average math score for students of each grade level (9th, 10th, 11th, 12th) at each school.

##Reading Scores by Grade
Create a DataFrame that lists the average reading score for students of each grade level (9th, 10th, 11th, 12th) at each school.

#Scores by School Spending
Create a table that breaks down school performance based on average spending ranges (per student).
Use pd.cut to categorize spending based on the bins.


**spending_bins = [0, 585, 630, 645, 680]**

**labels = ["<$585", "$585-630", "$630-645", "$645-680"]**

Use the scores above to create a DataFrame called spending_summary.

Include the following metrics in the table:

Average math score
Average reading score
% passing math (the percentage of students who passed math)
% passing reading (the percentage of students who passed reading)
% overall passing (the percentage of students who passed math AND reading)

# Scores by School Size
Use the following code to bin the per_school_summary.

**size_bins = [0, 1000, 2000, 5000]**
**labels = ["Small (<1000)", "Medium (1000-2000)", "Large (2000-5000)"]**

Use pd.cut on the "Total Students" column of the per_school_summary DataFrame.
Create a DataFrame called size_summary that breaks down school performance based on school size (small, medium, or large).

#Scores by School Type
Use the per_school_summary DataFrame from the previous step to create a new DataFrame called type_summary.
This new DataFrame should show school performance based on the "School Type".

## Summary 

For the analysis, The student data is merged with school data to have a better understanding of the School's academic performance
with various criteria like School Type,  Total Student Budget, Per student Budget.

From the District summary, For the total student strength of 39,170, there are 15 high schools in the district. 
The total budget allocated to the Schools is $24,649,428. The overall passing rate of the students who passed in both Math and English is 65.17.
 When comparing the individual subject results of the students, English has a higher passing rate than Math.

From the School summary, The District has an equal number of District  Schools and  Charter Schools, Whereas the student strength is
 higher in district schools than the Charter Schools.
The fund allocated per student for the District schools is higher than the Charter Schools.
When comparing the academic performance, the Charter Schools have a higher overall passing rate. 
That is first five highest performing schools are Charter schools and the first five bottom performing schools are District Schools.

# Conclusions
1. The budget spending doesn't affect the academic performance of the student. As seen in the data, the Schools with the lowest 
spending Schools has performed better than higher spending Schools.

2. When comparing the individual subject results, the Charter School has a higher passing rate in Math than the District Schools.
 This might have affected the overall passing rate of the District Schools which is lower than the Charter School.

3. In the overall passing rate, the Schools with small size perform better than the large size.
In other words, Charter Schools perform better than District Schools. 
However, We need more data to compare the District and the Charter Schools academic performance.
 4. Although there are an equal number of District and Charter Schools in the district, the public prefer to attend the District School 
than the Charter School.





