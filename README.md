# datafun-05-data-at-rest
## Files, Exceptions, and SQL

Get Started
Log in to your GitHub account. 
Create a new GitHub repo named datafun-05-data-at-rest. Follow conventions - use kebob, lower case, no spaces. 
Git clone your new repo into your Documents folder. 
Always ensure your repo has the basic files all our repos need:
a good README.md,
.gitignore
Copy these from previous repos as needed. This is done in a notebook - no need for logger. We'll show results in the notebook.
Update README.md to reflect the focus of this module. 
Authors examples: You're encouraged to use the authors examples for practice. Use the examples directly from your local IntroToPython directory - please DO NOT commit the author's work to your repo. 

## Task 1
Read and work through Chapter 9 - Files & Exceptions - understand the examples. 

9.1 Introduction
9.2 Files
9.3 Text-File Processing
9.3.1 Writing to a Text File: Introducing the with Statement
9.3.2 Reading Data from a Text File
9.4 Updating Text Files
9.5 Serialization with JSON
9.6 Focus on Security: pickle Serialization and Deserialization
9.7 Additional Notes Regarding Files
9.8 Handling Exceptions
9.8.1 Division by Zero and Invalid Input
9.8.2 try Statements
9.8.3 Catching Multiple Exceptions in One except Clause
9.8.4 What Exceptions Does a Function or Method Raise?
9.8.5 What Code Should Be Placed in a try Suite?
9.9 finally Clause
9.10 Explicitly Raising an Exception
9.11 (Optional) Stack Unwinding and Tracebacks
9.12 Intro to Data Science: Working with CSV Files
9.12.1 Python Standard Library Module csv
9.12.2 Reading CSV Files into Pandas DataFrames
9.12.3 Reading the Titanic Disaster Dataset
9.12.4 Simple Data Analysis with the Titanic Disaster Dataset
9.12.5 Passenger Age Histogram

## Task 2
Read and work through Chapter 17 - Big Data - understand the examples. 

17.1 Introduction
17.2 Relational Databases and Structured Query Language (SQL)
17.2.1 A books Database
17.2.2 SELECT Queries
17.2.3 WHERE Clause
17.2.4 ORDER BY Clause
17.2.5 Merging Data from Multiple Tables: INNER JOIN
17.2.6 INSERT INTO Statement
17.2.7 UPDATE Statement
17.2.8 DELETE FROM Statement
 

## Task 3 - Titanic Passengers (from 9.12 above)
Follow the instructions in 9.12.3 (starting pg. 346).
Don't work in interactive mode!
Instead complete the exercise in a Jupyter notebook. 
Perform the following subtasks.
Required: Include the title of the notebook, and your name and date at the top.
Required: Use Section headings in your Markdown to make it clear that each of these 6 sections are shown in your notebook. They should be numbered 1-6 and include the keyword shown below.
Recommended: Use titles and section headings in every notebook. Communication is important and clear organization is valuable.
Section 1-Load: Use pandas to read in the Titanic Disaster dataset csv file.
Section 2-View: Set the precision to 2 decimal places. View the head and tail of the file.
Section 3-Headings: customize the column headings.
Section 4-Describe: Use the DataFrame describe() function to calculate basic descriptive statistics for all numeric columns. 
Section 5-Survivors: Follow instructions to describe statistics for those who survived (titanic.survived == 'yes') - see the example. 
Section 6-Histogram: Use the DataFrame's hist() function to create a histogram for each numerical column.
Helpful Hints

The csv file is available on GitHub at https://raw.githubusercontent.com/pandas-dev/pandas/main/doc/data/titanic.csvLinks to an external site.
For more about using pandas with the titanic data set, see the pandas titanic tutorial hereLinks to an external site..
Notice that describe() provides different results for non-numeric data (e.g., unique, top, freq)
Enable matplotlib. If it doesn't work (e.g., in a notebook), try 
%matplotlib inline
 

Task 3 Output
Document your results.

execute the completed notebook before you commit and push to GitHub
 

## Task 4 - SQL (from 17.2 above)
Follow the instructions in 17.2.1 (starting pg 730) 
Don't work in interactive mode - use a notebook.
IMPORTANT: create the table using the books.sql script provided with the author files. 
On Windows, use PowerShell, on Mac use Terminal. (Generally for all commands we use in this course).
Try to populate your own database from the script. If you can't, download a populated books.db Download books.db.
In your Python code, import the sqlite3 module and use the connect function to create a connection to your database.
After running the script, there should be 3 tables: authors, author_ISBN, and titles. 
Import pandas as pd
Use pd options.display to set the max_columns to 10
Use pd read_sql fuction to select everything (*) from the authors table, then the titles table, then the author_ISBN table.
Section 1: SELECT. Complete 17.2.2 SELECT (1 query)
Section 2: WHERE. Complete 17.2.3 WHERE (3 queries)
Section 3: ORDER BY. Complete 17.2.4 ORDER BY (4 queries)
Section 4: INNER JOIN. Complete 17.2.5 INNER JOIN (1 query)
Section 5: INSERT INTO. Complete 17.2.6 INSERT INTO (2 queries)
Section 6: UPDATE. Complete 17.2.7 UPDATE (2 queries)
Section 7: DELETE FROM. Complete 17.2.8 DELETE FROM (2 queries)
Section 8: SELECT. Show your Final Results, SELECT * from each table and display the final state of each of the 3 tables.
Required: Include the title of the notebook, and your name and date at the top.
Required: Use Section headings in your Markdown to make it clear that each of these 8 sections are shown in your notebook. They should be numbered 1-8 and include the SQL keyword shown above. Use a heading before your the final results showing all 3 tables as well. 
 

Task 4 Output
Document your results.

execute the completed notebook before you commit and push to GitHub
Task 5. Push Repo to GitHub
Use VS Code to commit and sync (push) your repo to GitHub.

## Optional Task 6. Bonus
Start a new notebook.
Locate a unique csv dataset. 
Use pandas to import the csv dataset into a DataFrame.
Use the DataFrame commands to clean the data as needed and/or rename the columns.
Use the DataFrame describe() function to calculate basic descriptive statistics. 
Use the DataFrame hist() function to generate histograms for all numeric columns. 
Include the required heading at the top, and use section headings to tell your story with data. 
Execute the entire, professionally presented file and output to html. 
Git add, git commit, and git push the new content to your GitHub repo. 