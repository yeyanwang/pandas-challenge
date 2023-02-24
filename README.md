# PyCity Schools Analysis

The `PyCitySchools` directory contains a Jupyter Source File which reads in 2 datasets (`schools_complete.csv` and `students_complete.csv`) from the `Resources` folder and uses Pandas library to analyze the district-wide standardized test results. 

Pandas library was imported to help create DataFrames which show school standardize tests performance based on different varibles (such as school type, school size, spending per students, etc.)

**Findings:**


* Looking at Scores by School Size, small (< 1000) and medium (1000 - 2000) sized schools have higher average math and reading scores, and higher % in passing math, reading and % overall passing than the large (2000 - 5000) sized schools.

	| | Average Math Score	|Average Reading Score	|% Passing Math	|% Passing Reading	|% Overall Passing|	
  |---:      |     :---:      |     :---:      |    :---:      |     :---:      |    :---:      |
  |Small (<1000)	|83.821598	|83.929843	|93.550225	|96.099437	|89.883853|
  |Medium (1000-2000) |	83.374684	| 83.864438	| 93.599695| 96.790680	|90.621535|
  |Large (2000-5000) |	77.746417	| 81.344493	| 69.963361	|82.766634	|58.286003|

* Comparing Scores by School Type, students from charter schools have higher average math and reading scores, and higher % in passing math, reading and % overall passing than the students in district schools.
  | |Average Math Score	|Average Reading Score	|% Passing Math|	% Passing Reading|	% Overall Passing|
  |:---:      |     :---:      |     :---:      | :---:      |     :---:      |     :---:      |
  |Charter |	83.473852|	83.896421	|93.620830	|96.586489	|90.432244|
  |District |	76.956733	|80.966636	|66.548453	|80.799062	|53.672208|

* The top 5 Highest-Performing Schools (by % Overall Passing) are charter schools and the 5 Bottom-Performing Schools (by % Overall Passing) are district schools. However, there is substantial evidence that charter schools are typically smaller in school size than district schools. This may indicate that students in small-sized schools receive more individualized attention than students in large-sized schools, which might explain why charter schools perform better on the standardized tests.

  **Top 5 Highest-Performing Schools** 
    |  |School Type|Total Students|	
    |:---:      |     :---:      |     :---:      |
    |Cabrera High School|	Charter	|1858	|
    |Thomas High School	|Charter	|1635|	
    |Griffin High School|	Charter|	1468|
    |Wilson High School|	Charter|	2283|
    |Pena High School|	Charter|	962|
    
  
  **Bottom 5 Performing Schools** 
  	| |School Type|	Total Students|	 	
    |:---:      |     :---:      |     :---:      |
    |Rodriguez High School |	District |	3999 |	 
    |Figueroa High School |	District |	2949	 |  
    |Huang High School	|District	|2917 |
    |Hernandez High School	|District	|4635 |
    |Johnson High School	|District	|4761|

* Higher spending per student did not seem to yield better test results. Looking at the Spending Ranges (Per Student), students in the lowest spending range ("< 585") have better average math and reading scores, and higher % in passing math, reading and % overall passing than students in the other 3 higher spending ranges.

	|         | Average Math Score | Average Reading Score |	% Passing Math	| % Passing Reading |	% Overall Passing |
  |  ---:   |    :---:           |    :---:              |    :---:         |    :---:          |    :---:          |
  |<$585	  |83.455399           |	83.933814            |    93.460096     |	96.610877         |	90.369459         |
  |$585-630	|81.899826           |	83.155286	           |87.133538	        |92.718205	        |81.418596          |
  |$630-645	|78.518855           |81.624473              |	73.484209       |	84.391793	        |62.857656          |
  |$645-680	|76.997210           |	81.027843            |	66.164813     	|81.133951	        |53.526855          |
