# Data-Project-1

## Contributors
* Colin Henry

## Instructions
* Select the Run All button to execute the code.
* The first code block will install all necessary libraries needed for the following code.
* The second code block will do an API call to the OpenMeteo Weather Forecast API to get the data for various metrics for the last 7 days (hourly data). It will format the data into a panda dataframe with the proper column names and datetimes.
* The third code block will request the user to input the name of the static file to read in (CSV or JSON). It will then check the filetype and read it in accordingly, formatting it into a panda dataframe. It will then compute summaries on each of the static file and API data for number of records and columns. Next, it will clean the data and reformat the column names to ensure that both sources have the same formatting for the merge. It will merge the two into one dataframe, compute summaries on it, and then save the data as a sqlite database.
* The fourth code block will ask the user if they would like to remove or add a column from the database. It will then prompt them for the column name and if adding a column, then ask for a default value to assign. This will be saved in the sqlite database for data persistence. The user will also be asked what form of output data they want (CSV, JSON, or SQL), which will be done via converting the panda dataframe.
* The fifth code block will perform some data analysis by calculating the last 7 day period for each year from 2020 to 2025. It will then gather the metrics for each period and rename the columns to more understandable names with proper units. It will plot each of the metrics in their respective weather groups (temp, rainfall, snowfall, and wind) in barplot form with each year shown next to each other to visualize trends in the data.
