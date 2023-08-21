## CS 122B Team WJJ

### Contribution              
P1
Chengfeng Tang - Servlets + Json + Github + MySQL + Debug + Demo

Jingjing Wang - HTML + CSS + AWS + Jump Function + Project setup / management

P2
Chengfeng Tang - Servlet + Js + HTML + Github + MySQL + Debug

Jingjing Wang - HTML + Session/Session Storage + CSS + AWS + Project setup + Demo

We use Like%input% for all substring mathces(title,director,name) and 
COLLATEutf8mb4_general_ci for case insensitivity. Basically all string searche will return results that include the input anywhere in the string.

P3
Chengfeng Tang - reCAPTCHA + Prepared Statement + XML

Jingjing Wang - HTTPS + Encryption + Dashboard + DEMO

File names with prepared statements: DashboardServlet, insertion, LoginEmployeeServlet, LoginServlet, MovieListServlet, Payment, SingleStarServlet, SingleMovieServlet


All insertion Optimizations:
1. Batch Insertion: Instead of inserting records one by one, batch insertion allows the database to take a group of records and insert them at once. Significantly reduced the amount of overhead in establishing database transactions, which in turn greatly improved the speed of the operation.
2. Created index on table star(name) and movies(title). It significantly sped up the data retrieval operations by allowing the database to find the data associated with a particular value much more quickly. Indexing the 'name' column of the 'star' table and the 'title' column of the 'movies' table allows for faster retrieval of these entities.
3. Use efficient data structures to store and manipulate the data. Arrays allow for fast retrieval of elements at any index, while hash maps allow for fast retrieval of values associated with any given key. 
4. BadData: Keeping track of bad data or erroneous can help avoid repeating the same mistakes or wasting time on data that will not be useful. This involves keeping a list of records that have caused errors in the past or have been identified as incorrect or irrelevant.
5. NotFoundStars and NotFoundMovies: These act as caches for stars and movies that have been searched for but not found in the database. By keeping a record of these, the system can avoid wasting time on unsuccessful database queries. If the system tries to look up a star or movie that's not in the database, it can check this list first and avoid a potentially time-consuming database operation if the star or movie is listed there.


862,803 miliseconds without optimization

34,103 miliseconds after optimization


Inconsistent data reports: 

12115 Movies, inerted 11690, 52 duplicates, 425 inconsistent (contains typo or invalid data).

6862 Stars, inserted 5969.

inserted 8757 genres_in_movies

inserted 8698 stars_in_movies

12575 stars not found.

417 movies not found.

See reports for details.

P4
Chengfeng Tang - Full Text Search + Autocomplete + Fuzzy Search 
Jingjing Wang - Andriod + Demo


### Website Link  
https://wallamovie.store:8443/cs122b/login.html

### Demo Link 
https://youtu.be/QHrfIfA03q4

