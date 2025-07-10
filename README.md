# 🎬 Movie Analytics Dashboard (Power BI)
![](House.jpg)

## Introduction

This project analyzes a rich movie dataset using Power BI, with a focus on uncovering patterns in critical and audience reviews, production trends, and contributor impacts (directors, writers, actors). Through thoughtful data modeling, insightful visualizations, and interactivity, the dashboard delivers an engaging tool for data exploration and storytelling in the film industry.

---

## Skills and Concepts Demonstrated

- Power BI Desktop: Data modeling, visuals, bookmarks, slicers, drillthroughs, tooltips  
- Data Cleaning & Transformation: Power Query (split columns, unpivot, trim, replace values)  
- Data Modeling: Star schema design with fact and dimension tables  
- DAX: Custom measures and calculated columns  
- Data Visualization: Comparative charts, donut visuals, interactive tables  
- Insight Communication: Patterns, trends, and key performer evaluations  

---

## Problem Statement

The movie industry produces thousands of films annually. But what makes a movie stand out in terms of critical acclaim and audience reception? This project answers:

- Which contributors (director, writer, actor) have the most influence on ratings?  
- How do genres and studios perform over time?  
- What rating patterns exist across movie classifications?  
- What characteristics are shared by the most viewed or most acclaimed films?

---

## Modeling

### Data Preparation

- Loaded and referenced the original dataset as `Source` and disabled its load.  
- Renamed columns for clarity and consistency.  
- Created an index column for unique identification.

### Dimensional Modeling

- Duplicated the main dataset to create dimension tables for:
  - Genres
  - Directors
  - Writers
  - Actors
- Used delimiter splitting, unpivoting, and trimming techniques to normalize these tables.  
- Removed genre, director, writer, and cast columns from the main fact table.  
- Cleaned the "Movie Rating" column via value replacement.  
- Added a Date Table for time-based analyses.

---

## Visualizations

### Summary Dashboard

**KPIs:**
- Movie Count: 16,638
- Critic Count: 941,829
- Avg RT Score: 60.5
- Avg Audience Score: 60.5
- Avg Runtime: 102.39 mins
- Audience Count: 2.5 billion+

**Charts:**
- Clustered bar chart: Top 50 Movies by Audience Size and Avg RT Score  
- Column charts:
  - Year vs. Movie Count (1914–2020)  
  - Rating Category vs. Count  
  - Studio vs. Movie Count  

### Genre Page

- Stacked bar chart: Genre vs. Movie Count (Drama leads with 9,006 titles)  
- Donut charts:
  - RT Score vs. RT Score Remaining  
  - Audience Rating vs. Remaining  
- Table: Detailed movie-level metrics by genre  

### Director Page

- Line & Clustered Column Chart:
  - Directors by Movie Count and Average Ratings (e.g., Woody Allen, Spielberg, Hitchcock)  
- RT Fresh Threshold used as benchmark  
- Supporting donut charts and detailed movie table  

### Actor Page

- Analysis of prolific actors (e.g., Samuel L. Jackson, Bruce Willis)  
- Average critic and audience score comparison  
- Donut visuals and sortable data tables  

### Writer Page

- Highlights frequent screenwriters and their score trends (e.g., Coen Brothers, Woody Allen)  
- Line and bar combo chart with "Fresh" threshold  
- Donut visuals and accompanying table  

### Interactivity

- Slicers for Genre, Rating, Year, Contributor  
- Bookmarks for seamless page navigation  
- Drillthrough pages for deep-dive on specific films  
- Tooltips for contextual information on hover  

---

## Analysis

### Key Observations

- Top Studios: Paramount Pictures, Warner Bros., and Universal dominate in volume.  
- Genre Insight: While Drama leads in production volume, Action & Adventure and Animation films often score higher with audiences.  
- Audience vs Critic Score: Ratings are often not aligned; some films like Gladiator have moderate critic scores but high audience approval.  
- Contributor Impact:
  - Directors like Spielberg and Hitchcock consistently deliver high average scores.  
  - Actors such as Samuel L. Jackson and Robert De Niro appear frequently in top-rated films.  
  - Writers like Joel & Ethan Coen are notable for maintaining both high critic and audience scores.  

---

## Conclusion and Recommendations

### Conclusion

The analysis shows a complex but insightful relationship between film genre, contributors, and ratings. Audience scores don't always align with critical reviews, revealing the subjective nature of film reception. Certain directors, studios, and genres consistently produce content that resonates more deeply with audiences or critics.

### Recommendations

- Studios: Invest in genres like drama and adventure but track emerging trends in niche categories like anime and cult films.  
- Streaming Platforms: Use contributor-based recommendations to personalize content.  
- Marketers: Highlight director/actor past success as a value prop for new releases.  
- Analysts: Consider enhancing the model with box office data or user review sentiment for a fuller picture.

---
