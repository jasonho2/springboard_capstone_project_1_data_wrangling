# springboard_capstone_project_1_data_wrangling
Milestone report for springboard capstone project 1: data wrangling

OpenRefine is a powerful and useful tool for data cleaning, just noting that I used it for some cleaning.

Data wrangling steps:
  - Data cleaning: Using OpenRefine, I inserted 0 for missing values (dashes or blank) for the players without a 3-point shooting percentage. I also converted all values in the dataset to numbers with the exception of the players's name. This makes any further exploration and analysis easier to deal with using only ints and floats. I decided to leave the outliers for the player stats as they are. Other than the missing values the data was clean.
  - I merged two datasets using pandas: one that had player data and the year they were drafted and another with a target column indicating that the player has played in the NBA for at least five years. Joining on the Name column, I was able to merge to dataframes to one with year drafted and target five years. This is important for making separate dataframes to analyze: players who played for at least five years, players who did not play for five years, and players who have not yet been in the NBA for five years. 
  
  I will end up testing my model on the players who have not yet played in the NBA for five years based on the differences in the other two groups of players.
