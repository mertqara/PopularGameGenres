# VideoGameGenreShiftOvertime-DSA210Project

## Project Overview

In this project, I will analyse the correlation between video game genres and their release year in game industry. By analyzing the data, I want to understand how gaming industry preferences have shifted over time. By the end of my project, I hope to find out whether indie game companies or big corporations have played a role in the shift. Also, I will explore whether regional differences impact the popularity of certain genres. Do players in different parts of the world like different types of games?

---

## Motivation

This project really interests me because I have had a passion for games since my childhood and I would like to know how the industry shaped itself

1. **Personal Interest:**
    I love video games so this project is really exciting for me to work on.

2. **Data Analyze Skills:**
    I want to improve my data analysis skills. Therefore, using techniques which we learned in class hopefully help me to improve my data analysis skills.

3. **For my Future:**
   I also have a interest in game development not only playing it. These might be useful for me in the future in this sector.

---

## Dataset

This public dataset "Video Game Sales" includes some factors and popularity of video game genres. Also, the games which sold more than 100.000 copies are included.

- **Rank** - Ranking of overall sales

- **Name** - The games name

- **Platform** - Platform of the games release (i.e. PC,PS4, etc.)

- **Year** - Year of the game's release

- **Genre** - Genre of the game

- **Publisher** - Publisher of the game

- **NA_Sales** - Sales in North America (in millions)

- **EU_Sales** - Sales in Europe (in millions)

- **JP_Sales** - Sales in Japan (in millions)

- **Other_Sales** - Sales in the rest of the world (in millions)

- **Global_Sales** - Total worldwide sales

This is the link of the dataset: https://www.kaggle.com/datasets/gregorut/videogamesales


This public dataset "Top Video Games 1995-2021 Metacritic" includes games' metacritic scores and users scores.

- **Name** - The games name
  
- **Platform** - Platform of the games release (i.e. PC,PS4, etc.)

- **Year** - Year of the game's release

- **Metascore** - Metacritic's score on games

- **User Review** - Users' reviews on games

This is the link of the dataset: https://www.kaggle.com/datasets/deepcontractor/top-video-games-19952021-metacritic


This public data set "Popular Video Games 1980 - 2023" is similar to first dataset but contains recent games. Also, games genres are more comprehencive.

- **Name** - The games name

- **Year** - Year of the game's release

- **Publisher** - Publisher of the game

- **Rating** Average rating of the game

- **Genre** - Genre of the game

- **Review** - Number of reviews by users

- **Lists** The number of users listed this game

This is the link of the dataset: https://www.kaggle.com/datasets/arnabchaki/popular-video-games-1980-2023

---

## Data Analysis

### **1. Data Preprocessing**
For this project, I will use publicly available datasets that contains information on video game genres, release years, publishers, metacritic scores, and regional sales. 
- Cleaned and filtered data from public datasets from kaggle.
- Combining datasets with specific parameters.

### **2. Exploratory Data Analysis (EDA)**
After cleaning the data. I will perform Exploratory data analysis
- **Genre Distribution Over Time:** Identify which genres were most popular in different time periods.
- **Sales Trends:** Analyze whether certain genres perform better in sales.
- **Indie vs. AAA Impact:** Compare whether indie studios or major gaming companies drive genre shifts.
- **Regional Influence:** Examine if genre preferences vary by region based on sales data.

I will also visualize summary statistics and look for outliers or inconsistencies that may affect later analysis.

### **3. Correlation Analysis**
To find relationships between variables, I will conduct a correlation analysis between:
- **Genre vs. Release Year:** Check if some genres have become more or less common over time.
- **Game Ratings vs. Popularity:** Investigate whether higher-rated games contribute to long-term genre trends.
- **Major Company vs. Indie Company Influence:** Determine if major studios or indie developers have influenced the rise or fall of certain genres.
- **Regional Preferences:** Compare genre popularity across different regions to identify market differences.
This analysis will help determine whether certain factors have a statistically significant impact on video game trends.

### **4. Visualization**
To clearly show correlations between variables I will use various data visualation techniques:
- **Time Series Charts**
- **Heatmaps**
- **Bar Charts & Pie Charts**
- **Scatter Plots**
These visualizations will support me in my conclusions.
