# Movie Rating Platform
the Movie Rating Platform Dataset, which is one of the best for prep because it touches almost every real-world SQL concept: ratings, averages, joins, grouping, and window functions.
We’ll again use the same structure (Easy → Medium → Hard) and pattern alignment from our SQL concept map. Assumed tables:
* movies(movie_id, title, release_year, genre)
* users(user_id, name, join_date)
* ratings(rating_id, user_id, movie_id, rating, rating_date)
* reviews(review_id, movie_id, user_id, review_text, review_date)

-----
SQL Practice Set — Movie Rating Platform Dataset (30 Questions)

Level 1: Easy (Basics, Filtering, Aggregation)
Focus: SELECT, WHERE, ORDER BY, and simple COUNT, AVG.

1. List all movies released after 2020.
2. Find the total number of movies in the dataset.
3. Display all distinct genres available.
4. Count how many ratings each movie has received.
5. Find the average rating of each movie.
6. List the top 5 most recent movies by release year.
7. Show all users who joined before '2023-01-01'.
8. Display the total number of ratings submitted by each user.
9. Retrieve the movie(s) with a perfect 5-star rating.
10. Find the overall average rating across all movies.
 - Concepts used: SELECT, COUNT, AVG, GROUP BY, ORDER BY.

-----
Level 2: Medium (Joins, Grouping, Subqueries)
Focus: joins between movies ↔ ratings ↔ users, grouping, subqueries.

11. List each movie title with the name of the user who rated it and the rating value.
12. Find movies that have never received any ratings.
13. Retrieve the top 3 highest-rated movies (by average rating).
14. List users who rated more than 10 movies.
15. Find the average rating for each genre.
16. Show all users who reviewed at least one movie but didn’t rate it.
17. Find movies that have ratings above the overall average rating.
18. Display all movies that belong to the same genre as the movie “Inception.”
19. Show movies with both reviews and ratings made on the same day.
20. Find the most-rated genre by total number of ratings.
- Concepts used: INNER JOIN, LEFT JOIN, GROUP BY + HAVING, Subquery (IN, EXISTS).

-----

Level 3: Hard (Analytics, CTEs, Window Functions, Real-world Insights)
Focus: advanced logic, ranking, aggregates, and data storytelling.

21. Use a CTE to calculate the average rating per movie, then find those above 4.5.
22. Rank movies by their average rating within each genre (using RANK() OVER).
23. Find the top-rated movie per genre.
24. For each user, find their highest-rated movie.
25. Find users who consistently rate above the global average rating.
26. Calculate the average rating per year, ordered by year.
27. For each genre, show the total number of movies and their average rating.
28. Identify the most active reviewer (based on total reviews written).
29. Calculate the rating growth trend — compare average ratings per year using a window function (LAG() for previous year).
30. Create a view movie_insights containing:
* movie_id, title, avg_rating, rating_count, top_reviewer_name.
 - Concepts used:
* CTE
* Window Functions (RANK, ROW_NUMBER, LAG)
* Aggregates + Grouping
* Analytical queries with joins
  
-----

##  Setup Instructions

1. **Create the database**
   ```sql
   CREATE DATABASE movie_rating_platform;
   USE movie_rating_platform;


## Analysis

The documentation of the data analysis process is included in the file [*movie_rating_platform.sql*]()

## Summary

The project was done for the purpose of practice and to improve skills in SQL.

  
