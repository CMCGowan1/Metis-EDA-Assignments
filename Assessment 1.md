https://docs.google.com/forms/u/0/d/e/1FAIpQLScq2HoAOSuDLtBEaETVgheY1YR6IIc3DcbjFTC4a6TC5rZvvA/formResponse

Exploratory Data Analysis Part 1 V1.3
Total points
85/100
 
Email *
Cheryl@adventurex2.com
0 of 0 points
First Name *
Cheryl
Last Name *
McGowan
Python for EDA
25 of 30 points
 
1) What is a Pandas Series?
5/5
A 2-dimensional matrix
A 1-dimensional array
 
A sorting method
A numerical column
 
2) What does df.head() do in Pandas? Assume that df is a pandas DataFrame.
5/5
Displays the last few rows of the DataFrame
Displays a random subset of rows in the DataFrame
Displays the last few columns of the DataFrame
Displays the first few rows of the DataFrame
 
 
3) If a pandas DataFrame named df_measurements has a column called “weight”, what is returned by df_measurements.weight.tail(20)?
5/5
A DataFrame containing the last 20 rows of df_measurements
A Series containing the twentieth row of df_measurements
A Series containing the last 20 entries of the “weight” column
 
An error because this command is invalid
For the next 3 questions (4-6), consider the following scenario. Suppose the following pandas DataFrame is saved under the variable name df_quarterly_sales. It contains the quarterly sales volume for sales representatives who are based in either New York or Boston.

 
4) You realize that the 1200 units attributed to Becca in Q2 of 2020 was a data entry error; it should be 120 units instead. Which of the following commands would successfully (and without warning) replace that value in the original DataFrame `df_quarterly_sales`?
5/5
df_quarterly_sales.6.units = 120
df_quarterly_sales.iloc['units', 6] = 120
df_quarterly_sales[6]['units'] = 120
df_quarterly_sales.loc[6, 'units'] = 120
 
 
5) Same scenario as the above. You are interested in calculating the average number of units each sales_rep sells in a quarter, e.g. 105 for Quin, 90 for Anita, etc.. Which of the following statements would successfully complete this task?
5/5
df_quarterly_sales.groupby('sales_rep').units.mean()
 
df_quarterly_sales.groupby('units').sales_rep.mean()
df_quarterly_sales.sales_rep.mean().units
df_quarterly_sales.units.mean().sales_rep
 
6) Same scenario as above. The profit per unit sold depends on the city: $20 per unit in New York and $15 per unit in Boston. This information is stored in the following dictionary: prof_per_unit = {'New York': 20, 'Boston': 15}. You are interested in creating a new column that calculates the total profit for the number of units sold in each row of `df_quarterly_sales`. Which of the following statements would successfully complete this task?
0/5
df_quarterly_sales['profit'] = df_quarterly_sales.city.map(prof_per_unit) * df_quarterly_sales.units
df_quarterly_sales.profit = df_quarterly_sales.city.sum(prof_per_unit) * df_quarterly_sales.units
 
df_quarterly_sales['profit'] = df_quarterly_sales.city.agg(prof_per_unit) * df_quarterly_sales.units
df_quarterly_sales.profit = df_quarterly_sales.groupby(‘city’).apply(prof_per_unit) * df_quarterly_sales.units
Correct answer
df_quarterly_sales['profit'] = df_quarterly_sales.city.map(prof_per_unit) * df_quarterly_sales.units
SQL for EDA
60 of 70 points
 
7) Which of the following statements about databases is FALSE?
5/5
A database refers to a place to store data in an organized fashion
SQL is a query language primarily associated with non-relational databases
 
The structure of a relational database must be predefined, whereas the structure of a non-relational database can be dynamic
Data in a relational database is stored in table format, whereas data in a non-relational database can be stored in another format, such as dictionaries
 
8) Which of the following is NOT a common method for dealing with missing values in a table of data?
5/5
Removing the rows containing them
Imputing them with a column mean, median, or mode
Filling them with a standard value such as zero
Leaving them in when there are only a handful, as they won’t affect an analysis
 
 
9) Which of the following is NOT displayed in a data model?
5/5
Primary keys in tables
Foreign key relationships between tables
Number of rows available in each table
 
Column names and types for each table
 
10) Which of the following does NOT need to be defined when creating a table in SQL?
5/5
Name of the table
Name of the columns
Data type of each column
Minimum and maximum value of each numerical column
 
 
11) Which of the following statements about primary keys in SQL is FALSE?
5/5
A primary key value uniquely identifies a row of data
A table can only have one primary key
A primary key can consist of one column or multiple columns
A primary key can have NULL (blank) values
 
 
12) Which of the following statements about foreign keys in SQL is FALSE?
5/5
A table can have multiple foreign keys
A table’s foreign key uniquely identifies a row of data in that table
 
A foreign key in one table links to a primary key in another table
A table can have both a primary key and a foreign key
 
13) Suppose a SQLite table has been created using the following statement:
0/5
Captionless Image
Yes, this statement is always valid and will always execute successfully
Yes, as long as the student_id 12345 does not yet exist in the students table
No, because the birthday field is missing from the INSERT statement
No, because the value for the middle_name field cannot be NULL
 
Correct answer
Yes, as long as the student_id 12345 does not yet exist in the students table
 
14) Which of the following statements about the treatment of NULL values in SQL is TRUE?
5/5
NULL values are not allowed by default
NULL values are treated the same way as a False boolean
Aggregation functions in SQL treat NULL values as zeros
Adding “NOT NULL” when defining a column within a CREATE TABLE statement forces the column to always contain a value
 
 
15) Which of the following is NOT a type of SQL join?
5/5
Inner
Outer
Left
Dual
 
 
16) Which of the following statements about SQL JOINs is FALSE?
5/5
You can join a table with itself
An OUTER JOIN will never have NULL values in the results
 
You can join two tables on multiple columns that they have in common
RIGHT JOIN and LEFT JOIN can be used interchangeably by switching the order of the tables being combined
For the next 2 questions (17-18), consider these two tables:

 
17) If I did an INNER JOIN of the two tables on movie_id, how many rows would be in my output?
5/5
2
3
 
5
6
 
18) Same scenario as the above. If I did a LEFT JOIN of the two tables, specifically A LEFT JOIN B, how many rows would be in my output?
0/5
3
4
 
5
6
Correct answer
5
 
19) Which is the correct order of operations in SQL?
5/5
SELECT FROM WHERE GROUP BY ORDER BY HAVING LIMIT
SELECT FROM WHERE GROUP BY HAVING ORDER BY LIMIT
 
SELECT FROM WHERE ORDER BY GROUP BY HAVING LIMIT
SELECT FROM WHERE HAVING GROUP BY ORDER BY LIMIT
 
20) Which of the following statements about UNIONs and JOINs in SQL is FALSE?
5/5
It is possible to do a UNION on more than two tables
JOINs and UNIONs can be used interchangeably in SQL
 
The columns of the first table must match the columns of the second table exactly when performing a UNION on two tables
The columns of the first table can differ from the columns of the second table when performing a JOIN on two tables
This form was created inside of Kaplan.
Google Forms
