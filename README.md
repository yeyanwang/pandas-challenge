# pandas-challenge

The **PyCitySchools** directory contains a Jupyter Source File which reads in 2 datasets (**schools_complete.csv** and **students_complete.csv**) from the Resources folder and uses Pandas library to analyze the district-wide standardized test results. 

Pandas library helps to create DataFrames which show school standardize tests performance based on different varibles (such as school type, school size, spending per students, etc.)

**Findings:**
* According to Scores by Spending, higher spending per student did not seem to yield better test results. Looking at the Spending Ranges (Per Student), students in the lowest spending range ("< 585") have better average math and reading scores, and higher % in passing math, reading and % overall passing than students in the other 3 higher spending ranges.
* Looking at Scores by School Size, small (< 1000) and medium (1000 - 2000) sized schools have higher average math and reading scores, and higher % in passing math, reading and % overall passing than the large (2000 - 5000) sized schools.
* Comparing Scores by School Type, students from charter schools have higher average math and reading scores, and higher % in passing math, reading and % overall passing than the students in district schools.
* The top 5 Highest-Performing Schools (by % Overall Passing) are charter schools and the 5 Bottom-Performing Schools (by % Overall Passing) are district schools. However, there is substantial evidence that charter schools are typically smaller in school size than district schools. This may indicate that students in small-sized schools receive more individualized attention than students in large-sized schools, which might explain why charter schools perform better on the standardized tests.
