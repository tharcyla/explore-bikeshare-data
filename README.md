### Date created
February 10, 2022

### Project Title
Explore US Bikeshare Data 

### Description
This project was undertaken as part of Udacity's Programming for Data Science with Python.

It mainly uses Python to understand U.S. bikeshare data using data
provided by [Motivate](https://www.motivateco.com/).

The script is able to calculate statistics and build an interactive environment.
In this interactive environment, raw user input as answers to a few questions will 
change the results: 
1. The city the user would like to see data from (there are 3 cities with available data);
2. Whether the user wants to filter by month, day, or both;
3. (If they choose month) which month;
4. (If they choose day) which day;
5. (If they choose both) which month and day.

Afterwards, the script will: 
- Filter the data based on the answers; 
- Display statistical data for the user;
- Ask whether they want to see raw data displayed (5 lines at a time);
- Ask whether they want to start again or exit. 

### Files used
data/chicago.csv

data/new_york_city.csv

data/washington.csv

### Credits
- I used the [Pandas documentation](https://pandas.pydata.org/docs/index.html) page  a lot,
especially on how to handle the [to_datetime function](https://pandas.pydata.org/docs/reference/api/pandas.to_datetime.html) and extract the month and day of the week using the [dt.month_name()](https://pandas.pydata.org/docs/reference/api/pandas.Series.dt.month_name.html) and [dt.day_name()](https://pandas.pydata.org/docs/reference/api/pandas.Series.dt.day_name.html) methods.

- I decided to allow the user to filter the DataFrame by both the month and day, but I ran into some errors while trying to get the mode() over those two columns.
A [StackOverflow](https://stackoverflow.com/questions/55719762/how-to-calculate-mode-over-two-columns-in-a-python-dataframe) discussion and a [Kite](https://www.kite.com/python/answers/how-to-filter-a-pandas-dataframe-by-multiple-columns-in-python) post helped me achieving that.

- In addition to Pandas and Numpy, the Udacity reviewer kindly recommended I use 
Tabulate to better display raw user data. 

- Afterwards, I had the idea to search how to create a requirements.txt file using conda. [Conda documentation](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html)
helped me generate the file.