# Final-Project-Tableau

## Project/Goals
My goal is to present a revolutionary dashboard designed to empower football coaches, facilitating seamless team selection and providing in-depth insights for a comprehensive understanding of opposing teams. Elevate people's coaching experience and optimize their strategies with ease.

## Process

# A) Data Cleaning
1. Connect the data with no issue.
2. 'Date-Time' tyoe of data is missing.
3. Three columns were deleted right away as I didn;t find any value: PHOTO, FLAG & CLUB LOGO.
4. NATIONALITY column was of string type. I casted it into Geographic role.
5. By doing a COUNT(Nationality) + PlayerName I found duplicates. 52 duplicates were removed in Excel.
6. Split the 'Preferred Position' column.


# B) Data Wrangling in Python
1. I found out that there were countries with a lot of players (such as England with over 1600) whereas other countries contain as little as less than 10 players. This would affect my results so I decided the following:
  i. Keep countries with at least 50 players.
  ii. Keep only the best 50 players per country using the 'Overall' column as parameter.

 2. I exported the new dataframe into a csv file. The csv and juoyter notebook can be found attached in this repo.

# C) Data Wrangling in Tableau
1. Created several Calculated Fields (such as GK skills, GK stats, and many more) with the stats I believe are the most important for each position in the field in order to find out who the best players for each position were.
2. Implemented filters to inject dynamism into the dashboard.

## Results

As I imagined myself stepping into a football coach's shoes, a bunch of questions popped into my head. Like, "What's the best combo for my dream team? Can players perform in different spots on the field? And if they switch it up, how's it going to affect their game?" Also, what about the other teams? Are they bringing their A-game, or are we in for an easy win? I'm looking to break it down by positions, such as goalies, defenders, midfielders, and attackers.

In the end, I crafted a nice dashboard that serves as a must-have tool for any football coach looking to up their game and excel in their role.


## Challenges 
Visuals in Tableau Desktop and in Tableau Web sometimes are very different, like sizes, chart positions, and many more.

## Future Goals
I would like to work more on filters and in calculating the average of the team stats when we sub one player for another one.
