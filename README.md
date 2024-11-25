# Python-capstone
The project consists of ABC company's Employees dataset which consists of 458 rows and 9 columns. Dataset includes details of all the employees across 29 different teams. Using Python libraries such as pandas, numpy, matplotlib, seaborn and various python functions, analysed and visualised the employee dataset to get many valuable and meaningful insights.


## Preprocessing

There were about 2 percent null values in Salary column and 18 percent null values in college column. 
Replaced null values of salary using fillna function with median of salary.
replaced null values of college with mode of the college column . 
height column included inappropriate values. replaced then with random values ranging 150 to 180.

## Analysis tasks:
### 1.To determine employee distribution across each team and calculate   the percentage split relative to the total number of employees. 

* Found the distribution of employees across each team using value counts() function.
* Created a data frame Employee with the result. Using formula, determined relative percent of each team and added to Employee as a new column.

#### Graphical represntation:
Used displot to visualise the result. As the data contained discrete values, used number of employees in x-axis and represented their relative percent as hues.

#### Insights Gained:
Most of the teams have employee distribution of 3.275 which is about 15 employees. only 2 teams	 have 18 and 19 employees. Another 2 teams with 14 and 3 teams with 16 Employees. Employee distribution across teams is near to equal , between 3% to 4%.

### 2.Segregate the employees bases on positions

Created a data frame with value counts of the column position, thus giving a table with position and the number of employees in each position.

#### Graphical Represntation:
As the graph includes one categorical and one numerical value , used barplot in seaborn to visualise the result, giving position in x-axis and number of employess in y-axis.

#### Insights gained:
Highest number of employees are in position SG . then comes PF with 100 ,PG, SF 
and position C at the last. From the graph, it is visible there is not a big difference in distribution of employees across various positions. All the positions occupy nearly 80 and more employees.

### 3.Identify the predominant age group.
To find most common age group, used mode function on the age column, which resulted 24 as the value.

#### Graphical Represntation:
To represent graphically, created a data frame with age and value counts. As both values are continuous values, used scatterplot in matplotlib with Age in x-axis and Count in y_axis.

#### Insights gained:
About 47 employees belongs to age 24 . 46 employees with age 25. it is very clear that most of the employees belongs to the age group of 23 - 30, with more than 20 employees in each age . Number of employees greater than 30 are less than 15 in each age group. Youngest employee is of age 19 and oldest employee is of age 40.

### 4.Team and position with the highest salary expenditure.

Using max function, found the highest salary. with the result found, using pandas filtering option, filtered out the team and position with the highest salary.

#### Graphical Representation:
Created data frame of top 10 salaries with their teams, positions and salary. from the new data frame, created a scatterplot in seaborn with salary in x-axis, teams in y-axis and position as hue. thus representing three variables in a single graph.

#### Insights Gained:
Employee in team Los Angeles Lakers with SF position has the highest salary 250000000.First three positions in top 10 salaries belongs to employees in SF position. Highest salaries come in the range of 20M to 25M.

### 5.Correlation between Age and Salary.
Created a data frame with age and salary and used corr() function on the newly created data frame. 

#### Graphical representation:
used lmplot to represent correlation of Age and salary, which can help to show even a small variance using regression line. lmplot has Age in x-axis and salary in y axis.

#### Insights gained:
Age and salary has a slight positive correlation. As age increases salary also increases. from scatterplot, values are more scattered to top as the age increases. Regression line clearly depicts the correlation between age and salary.

## Conclusion:
In ABC company, each team constitutes of 3 to 4 percent of employees. Most of the employees belongs to age 23-30 . There is a slight increase in salary as the age of employee increases. employees are distributed nearly same across different positions with each position having 80 employees and more.
Employee in SF position in the team Los Angeles lakers has the highest salary.





