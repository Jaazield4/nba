# nba

### Overview
This repository will serve as a template to be used to analyze current players and teams within the nba. This analysis is for personal use and will be used for practice. The goal is to create visuals such as scatter plots and shot charts
to depictate play of an NBA team or player. 

### Libraries used
The main focus of the nba_data_generator is to take statistics that are pulled from the nba_api to create the charts using matplotlib.
- Pandas
- Matplotlib
- nba_api
- numpy
- seaborn

### Getting Team and Player Data
To begin first pull the data from every NBA team by using the nba_api endpoint "from nba_api.stats.static import teams" which allows to view all 30 teams. However, this will present the teams data as a dictionary so to be easier 
to read and analyze we turn the data into a pandas dataframe using pd.DataFrame.from_dict('dict'). This should provide the following result.

![image](https://github.com/Jaazield4/nba/assets/85451089/18ea23e9-d83b-4860-b08d-7fb99dd9a581)

After receiving the team data, the focus is turned to retrieving player data. To retreive this data the endpoint is from nba_api.stats.static import players. And similar to the team data this must also be turned into a dataframe to
provide the following table

![image](https://github.com/Jaazield4/nba/assets/85451089/95bbfba7-5997-4a67-b1e5-f5d87effadc2)


### Creating A Shot Chart
Creating a shot chart requires the use of matplotlib, the nba_api, and seaborn. This is done by creating an accurate image of a half court following by layering a scatterplot on top. To create an accurate diagram of a basketball court
the following code snippet was used from bradley fay. The following code is used to get the data for a specific nba player.

![image](https://github.com/Jaazield4/nba/assets/85451089/e9cc8f24-6a0c-49da-8e32-1f743526c6ab)

This will be used to create the scatterplot that will be merged with the basketball half court function using the following snippet and result.

![image](https://github.com/Jaazield4/nba/assets/85451089/0abe5499-9c28-4c82-bf35-04852023d882)

This particular chart shows the shot selection as well as the makes and misses of Jimmy Butler during game 1 and 2 of the 2023 NBA Finals vs. the Denver Nuggets.

### What's Next
Following creating a simple shot chart, is going to be making the visuals stand out further by adding color background and written reports that will help translate the meaning behind these results.
