# Netflix EDA Data Analysis-
This project just focuses on using Power Query and Power BI to create the dashboard.
## Data from Kaggle - <a href = “https://www.kaggle.com/datasets/shivamb/netflix-shows?resource=download”>
## KPI Questions
These Key Performance Indicator (KPI) questions are designed to analyse different aspects of the Netflix content library.

Content Growth and Curation KPIs:
•	Content Volume: What is the total number of titles available on the platform?
•	Content Mix: What is the ratio of movies to TV shows in the current content library?
•	Annual Releases: How many titles were added each year, and what is the trend of content acquisition over time?
•	Genre Diversity: What are the top 5 most common genres by the number of titles?
•	Director Contribution: What is the total number of unique directors represented in the library?
## Audience and Accessibility KPIs:
•	Content Ratings: What is the most prevalent content rating on the platform (e.g., TV-MA, TV-14)?
•	Geographic Distribution: Which countries have the highest number of shows and movies available?
•	Content Age: What is the age range of the content library, from the earliest to the most recent release date?
________________________________________
## Data Cleaning Steps
The following steps were taken using Power BI Query to prepare the data for analysis:
•	Column Profiling: A preliminary review of the data columns was conducted to understand their characteristics.
•	Setting Headers: The headers were set to be the first row of data.
•	File Fixes: The CSV file was manually corrected to address a specific data issue, such as "William Wyler" being incorrectly listed as a type.
•	Dealing with Missing Values:
o	Director: The strategy for the director column was to fill missing values with "no director." The more complex method of using cast members to find directors was deemed unreliable.
o	Country: For missing country data, the assumption was made that the titles were produced in the United States, given that 31% of the movies were made there, and only 10% of the values were missing.
•	Changing Data Types:
o	Date added was changed to a date format.
o	release_year was changed to a whole number.
o	duration was converted to minutes using a conditional column and an if-else statement.
•	Splitting / Extracting Data:
o	A new Excel file was created for category mapping of the listed_in column.
o	The id and listed_in columns were used for category mapping.
o	The listed_in column was split using a comma delimiter to create separate rows for each genre.
o	The data was trimmed to remove extra spaces.

