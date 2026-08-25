# Netflix movies and TV shows Data Analysis using SQL

![Netflix Logo](https://github.com/manishshar1204-coder/Netflix_sql_project/blob/main/Logo)


# Netflix Movies & TV Shows – SQL Data Analysis

## Overview
End-to-end SQL analysis of the Netflix content catalog (~8,800 titles) to answer 15 real-world business questions covering content strategy, regional distribution, genre trends, and content classification. Built to simulate the kind of ad-hoc reporting and analytical requests a Business/Data Analyst would handle for a content or product team.

## Dataset
-**Dataset Link:[movies dataset] https://www.kaggle.com/datasets/shivamb/netflix-shows?resource=download
- **Source:** Netflix Movies and TV Shows dataset (`NETFLIX.csv`)
- **Rows:** ~8,800 titles
- **Columns:** show_id, type, title, director, cast, country, date_added, release_year, rating, duration, listed_in (genre), description

## Tools Used
- PostgreSQL
- SQL: aggregations, window functions, string parsing (`UNNEST`, `STRING_TO_ARRAY`, `SPLIT_PART`), CTEs, date functions, `CASE` logic

## Business Problems Solved
1. Count of Movies vs. TV Shows
2. Most common content rating by type
3. Movies released in a specific year
4. Top 5 countries by content volume
5. Longest movie by duration
6. Content added in the last 5 years
7. Filmography lookup by director
8. TV shows with more than 5 seasons
9. Content count by genre
10. Top 5 years by average content release share in India
11. All documentary titles
12. Content missing director information
13. Actor filmography count within a time window (e.g., last 10 years)
14. Top 10 actors by movie count in India-produced content
15. Content classification (e.g., "Good"/"Bad") based on keyword presence in description

Full queries and comments: [`solution.sql`](./solution.sql)

## Key Insights
- Movies significantly outnumber TV Shows in the overall catalog.
- A small set of countries (led by the US and India) account for a disproportionate share of total content.
- Genre and keyword-based classification can be done entirely in SQL without external NLP tooling, using pattern matching and `CASE` logic — useful for quick content audits.

## How to Run
1. Create the `netflix` table using the schema in `solution.sql`.
2. Load `NETFLIX.csv` via `COPY` (update the file path to your local location).
3. Run each numbered query independently — they are structured as standalone business questions.

## Author
Manish Sharma — PGDM (Data Science & Business Analytics), IIBS Bangalore




