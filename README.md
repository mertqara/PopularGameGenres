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

---

## Data Analysis

### **1. Data Preprocessing**
For this project, I will use publicly available datasets that contains information on video game genres, release years, publishers, metacritic scores, and regional sales. 
- Cleaned and filtered data from public datasets from kaggle.
- Combining datasets with specific parameters.

### **2. Exploratory Data Analysis (EDA)**
After cleaning and combining the data. I will perform Exploratory data analysis
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
- **Bar Plot**
- **Line Plot**
- **Scatter Plot**
- **Boxplot**
- **Stacked Bar Plot**
These visualizations will support me in my conclusions.

## **Exploratory data analysis**

### **1. Genre Distribution Over Time**

**Purpose:** See how genre popularity changed by decade.

**Plot Used:** Bar

![Image](https://github.com/user-attachments/assets/3e3c1001-d738-4844-9018-c143c5244944)

### **2. Sales Trends by Genre**

**Purpose:** Identify which genres generate the most average global sales.

**Method:** Calculated average Global Sales per genre.

**Plot Used:** Bar Plot

![Image](https://github.com/user-attachments/assets/29caf722-40cd-4af1-8db2-0539486342ed)

### **3. Indie vs AAA Impact on Sales**

**Purpose:** Compare sales performance between AAA studios and Indie studios.

**Method:** Classified games as AAA or Indie and compared Global Sales.

**Plot Used:** Boxplot

![Image](https://github.com/user-attachments/assets/6818d351-758f-412b-a715-c565fa31ad5d)

### **4. Regional Influence by Genre**

**Purpose:** Analyze how genre preferences vary by region (NA, EU, JP, Other).

**Method:** Summed sales by genre and region.

**Plot Used:** Stacked Bar Plot 

![Image](https://github.com/user-attachments/assets/78c37f5a-a45a-4993-88ce-420ceb6b48d5)

## **Correlation Analysis**

### **1. Genre vs Release Year**

**Purpose:** Explore how different genres evolved over decades.

**Method:** Grouped game releases into decades and counted games by genre.

**Plot Used:** Line Plot

**Findings:** Shooter and Action genres grew rapidly after 2000; Platformers declined.

![Image](https://github.com/user-attachments/assets/e0bca4e2-4cd7-4f6f-a877-ebc9e16fda7b)

### **2. MetaScore vs Global Sales**

**Purpose:** Investigate if games with higher critic scores (MetaScore) sell better.

**Method:** Correlated MetaScore with Global Sales using scatter plot and regression line.

**Plot Used:** Scatter Plot with Regression Line (scatterplot + regplot).

**Findings:** Weak positive correlation (r ≈ +0.24) — critic reviews slightly impact sales.

![Image](https://github.com/user-attachments/assets/64927566-be5a-41a8-b613-b451bd759f60)

![Image](https://github.com/user-attachments/assets/c81885f5-fb39-4203-a438-cf039caa62ac)

### **3. UserReview vs Global Sales**

**Purpose:** Check if user ratings affect sales.

**Method:** Correlated UserReview scores with Global Sales.

**Plot Used:** Scatter Plot with Regression Line

**Findings:** Almost no correlation (r ≈ +0.03) — user satisfaction does not predict sales.

![Image](https://github.com/user-attachments/assets/b70ad3f6-4495-4daa-8777-cdbcfc922328)

![Image](https://github.com/user-attachments/assets/45432263-537e-4007-8127-9ec980ed4574)

![Image](https://github.com/user-attachments/assets/6750862a-0533-4a18-a357-98030c05797d)

## **Hypothesis Testing**

### **1. AAA vs Indie Global Sales**

**Purpose:** Test if AAA games sell significantly more than Indie games.

**Method:** Independent Samples t-test comparing Global Sales of AAA vs Indie games.

**Plot Used:** Boxplot (during EDA), statistical t-test (hypothesis testing).

**Result:** p-value ≈ 1.087e-103 → Significant difference

*-*          t-statistic = 22.0724

*-*          Cohen’s d = 0.419

AAA games sell significantly more.

### **2. High vs Low MetaScore Global Sales**

**Purpose:** Test if games with higher MetaScores (>80) sell more than lower-rated games.

**Method:** Independent Samples t-test comparing Global Sales of High vs Low MetaScore games.

**Plot Used:** Scatter plot (during correlation analysis), statistical t-test (hypothesis testing).

**Result:** p-value ≈ 4.585e-41 → Significant difference

*-*         t-statistic = 13.7427

*-*         Cohen’s d = 0.443

Higher-rated games sell more.

### **3. Japan Sales vs Global Sales**

**Purpose:** Test if sales in Japan differ significantly from global sales

**Method:** Independent Samples t-test comparing Japan Sales vs Global Sales.

**Plot Used:** Stacked Bar plot (during regional EDA), statistical t-test (hypothesis testing).

**Result:** p-value ≈ 1.247e-208 → Significant difference

*-*         t-statistic = -31.2171

*-*         Cohen’s d = -0.355

Japan’s gaming market is statistically different from the global market and their favorite genre is role-playing as we can observe it from the plots.

## **Machine Learning Techniques**

### **1. Linear Regression**

Used Linear regression to make a simple model that tries to find a straight-line relationship between each feature (like review score or genre) and the sales.

Linear Regression served as a clean and simple baseline. It required dropping rows with missing values, but it still explained ~63% of the variance in global sales using only game metadata.

R² on test (dropping NaNs): 0.6267584485130828

### **Scatter Plot**

![Image](https://github.com/user-attachments/assets/a5388765-5a33-4b2b-9586-045553d37c28)

### **Bar Chart**

![Image](https://github.com/user-attachments/assets/37617bf1-c032-4c97-9557-2ca77f861964)

### **Confusion Matrix**

![Image](https://github.com/user-attachments/assets/071fd46f-6774-471f-b02b-f37a09539ed8)

### **Random Forest Regressor**

Initially appeared extremely accurate, with an R² score of 0.994 and very low error. However, this was due to the model using regional sales data such as (NA_Sales, EU_Sales) which when summed form the actual Global_Sales. This means the model was essentially adding up parts of the answer and making its predictions unrealistic for practical use.

R² score: 0.9941
RMSE (on log sales): 0.0494

## **Bar Chart**
![Image](https://github.com/user-attachments/assets/50af78c9-c959-4aa2-8398-ccc7c348a567)

## **Histogram**
![Image](https://github.com/user-attachments/assets/09520461-16da-45e6-b423-1de74f8daff7)

### **Gradient Boosting Regressor**

It provided the most trustworthy results. It handled missing values automatically and used only valid features such as genre, MetaScore, UserReview, studio type, and release year without relying on any part of the target variable. Despite this, it achieved an R² of 0.532, meaning it could explain over 53% of the variation in game sales based solely on a game's metadata.

R² score: 0.5322
RMSE (log sales): 0.3600

### **Histogram**
![Image](https://github.com/user-attachments/assets/9bfc4852-dd68-4127-9e74-3b02768ad458)

### **Scatter Plot**
![Image](https://github.com/user-attachments/assets/d8287024-af6f-450a-b5c1-fa23c4b117e4)











