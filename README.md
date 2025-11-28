🚀 SQL Project – Video Game Sales Analysis

📖 Project Overview

This project explores global video game sales using SQL. The goal was to uncover what drives game popularity and revenue performance across consoles, genres, and regions.

📂 Dataset
The dataset contained rich attributes:
- Game Titles
- Consoles (PS2, PS3, PS4, Xbox 360, etc.)
- Genres (Action, Shooter, Sports, etc.)
- Publishers & Developers
- Critic Scores
- Regional Sales (North America, Europe, Japan, Others)
- 
🔑 Key Insights
- Top-Selling Games & Publishers – Identified leaders by total and regional sales
- Genre-Wise Performance – Action, Shooter, and Sports dominated global charts
- Console Comparison – Lifetime sales across PS2, PS3, PS4, Xbox 360, and more
- Regional Breakdown – Sales trends in NA, Europe (PAL), Japan, and Others
- Critic Score Impact – Correlation between ratings and sales performance
- Year-Wise Trends – Peak release years and declining patterns
- Dynamic Filtering – Used WHERE, GROUP BY, HAVING, and JOINs for flexible exploration
- 
🛠️ SQL Skills Practiced
- Complex JOINs
- Aggregations with SUM, AVG, COUNT
- Subqueries for advanced filtering
- Performance optimization with indexes
- Query structuring for readability

📊 Sample Queries

-- Top 10 best-selling games globally
SELECT game_title, SUM(global_sales) AS total_sales
FROM video_game_sales
GROUP BY game_title
ORDER BY total_sales DESC
LIMIT 10;

-- Genre-wise performance
SELECT genre, SUM(global_sales) AS total_sales
FROM video_game_sales
GROUP BY genre
ORDER BY total_sales DESC;
