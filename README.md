# data_analysis_task_3

## SQL Data Analysis Project

## Overview
This project demonstrates my skills in SQL by working through key steps, from database creation to advanced query writing. The goal was to analyze and manage data effectively while exploring SQL functionalities.

## Steps Taken
- Database Creation:- Designed and created a database to store structured data.

- Table Management:- Built tables, including a secondary table derived from the primary dataset.

- Query Writing:- Wrote both basic and advanced queries to analyze data:- Filtered, aggregated, and grouped data.

- Applied techniques like subqueries for deeper insights.

- Joins:- Used INNER JOIN to combine data from multiple tables effectively.

- Indexing:- Created indexes on critical columns like Artist to optimize query performance.

## Challenges Faced:- 
Encountered issues while creating views and indexing and learned the importance of managing duplicates and query testing.

## 2 queries didn.t worked properly.

Query 1: Create a View
CREATE VIEW vibrant_playlist AS
SELECT Title, Artist, Energy, Danceability
FROM spotify_music_data
WHERE Energy > 0.8 AND Danceability > 0.7;

- The base table spotify_music_data may not contain rows that meet the specified conditions, resulting in an empty view when queried.

Query 2: Create an Index
CREATE INDEX idx_artist ON spotify_music_data(Artist);

Because while the query executed successfully, it showed "0 rows affected", which is expected behavior because creating an index doesn’t directly affect data rows—it only improves query performance.

## Key Takeaway:
I am just a beginner and this was my first time using mysql so i took help from youtubes in understanding queries and then write them, but i have a learned a lot from cleaning raw data in Excel to exploring advanced SQL features like views and indexes.
