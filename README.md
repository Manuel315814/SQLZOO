# SQLZOO

# SELECT basics ####

- **1. SELECT basics **
```
solution: 
SELECT population FROM world
  WHERE name = 'Germany'
```
- **2. SELECT basics **
```
solution:
SELECT name, population FROM world
  WHERE name IN ('Sweden', 'Norway', 'Denmark');
```
- **3. SELECT basics **
```
solution:
SELECT name, area FROM world
  WHERE area BETWEEN 200000 AND 250000
```
# SELECT basics Quiz ####
- **1. SELECT basics Quiz **
![Captura de pantalla 2025-03-16 201848](https://github.com/user-attachments/assets/2fe6e13f-a645-4c0f-9037-d1be453a9d6f)
- **2. SELECT basics Quiz **
![Captura de pantalla 2025-03-16 203911](https://github.com/user-attachments/assets/3e0451c6-2247-47b0-aa70-02152a8e7186)
- **3. SELECT basics Quiz **
[![Captura-de-pantalla-2025-03-16-201923.jpg](https://i.postimg.cc/wMQw97RP/Captura-de-pantalla-2025-03-16-201923.jpg)](https://postimg.cc/2L3QwjwF)
- **4. SELECT basics Quiz **
![Captura de pantalla 2025-03-16 204012](https://github.com/user-attachments/assets/89587bfe-f072-4bfb-a957-5cb902430b9b)
- **5. SELECT basics Quiz **
![Captura de pantalla 2025-03-16 204051](https://github.com/user-attachments/assets/78abb69d-a35b-49ca-8895-f2a1a0c99c70)
- **6. SELECT basics Quiz **
![Captura de pantalla 2025-03-16 201938](https://github.com/user-attachments/assets/f51995ca-e2e4-48de-b416-5c7bdc7d8d62)
- **7. SELECT basics Quiz **
![Captura de pantalla 2025-03-16 201943](https://github.com/user-attachments/assets/838609ad-5d73-425d-9b3c-65fe7f7e1567)

# SELECT names #
- **1. SELECT names **
```
solution:
SELECT name FROM world
  WHERE name LIKE 'Y%'
```
- **2. SELECT names **
```
solution:
SELECT name FROM world
  WHERE name LIKE '%Y'
```
- **3. SELECT names **
```
solution:
SELECT name FROM world
  WHERE name LIKE '%x%'
```
- **4. SELECT names **
```
solution:
SELECT name FROM world
  WHERE name LIKE '%land'
```
- **5. SELECT names **
```
solution:
SELECT name FROM world
  WHERE name LIKE 'C%ia'
```
- **6. SELECT names **
```
solution:
SELECT name FROM world
  WHERE name LIKE '%oo%'
```
- **7. SELECT names **
```
solution:
SELECT name FROM world
  WHERE name LIKE '%a%a%a%'
```
- **8. SELECT names **
```
solution:
SELECT name FROM world
 WHERE name LIKE '_t%'
ORDER BY name
```
- **9. SELECT names **
```
solution:
SELECT name FROM world
 WHERE name LIKE '%o__o%'
```
- **10. SELECT names **
```
solution:
SELECT name FROM world
 WHERE length (name)=4
## Harder Questions ##
```
- **12. SELECT names **
```
solution:
SELECT name
  FROM world
 WHERE name=capital
```
- **13. SELECT names **
```
solution:
SELECT name
  FROM world
 WHERE capital LIKE '% City'
```
- **13. SELECT names **
```
solution:
SELECT capital, name
FROM world
WHERE
  capital LIKE CONCAT('%',name,'%')
```
- **14. SELECT names **
```
solution:
SELECT capital, name
FROM world
WHERE
  capital LIKE CONCAT('%',name,'%')
AND 
   length(capital)>length(name)
```
# SELECT from world #
- **1. SELECT from world **
```
solution:
SELECT name, continent, population FROM world
```
- **2. SELECT from world **
```
solution:
SELECT name 
FROM world 
WHERE population >= 200000000;

```
- **3. SELECT from world **
```
solution:
SELECT name, gdp / population AS per_capita_gdp
FROM world
WHERE population >= 200000000;
```
- **4. SELECT from world **
```
solution:
SELECT name, population / 1000000 AS population_millions
FROM world
WHERE continent = 'South America';
```
- **5. SELECT from world **
```
solution:
SELECT name, population
FROM world
WHERE name IN ('France', 'Germany', 'Italy');
```
- **6. SELECT from world **
```
solution:
SELECT name
FROM world
WHERE name LIKE '%United%';
```
- **7. SELECT from world **
```
solution:
SELECT name, population, area
FROM world
WHERE area > 3000000 OR population > 250000000;
```
- **8. SELECT from world **
```
solution:
SELECT name, population, area
FROM world
WHERE (area > 3000000 AND population <= 250000000) 
   OR (population > 250000000 AND area <= 3000000);
```
- **9. SELECT from world **
```
solution:
SELECT name, 
       ROUND(population / 1000000, 2) AS population_millions, 
       ROUND(gdp / 1000000000, 2) AS gdp_billions
FROM world
WHERE continent = 'South America';
```
- **10. SELECT from world **
```
solution:
SELECT name, 
       ROUND(gdp / population, -3) AS per_capita_gdp
FROM world
WHERE gdp >= 1000000000000;
```
- **11. SELECT from world **
```
solution:
SELECT name, capital
FROM world
WHERE LENGTH(name) = LENGTH(capital);
```
- **12. SELECT from world **
```
solution:
SELECT name, capital
FROM world
WHERE LEFT(name, 1) = LEFT(capital, 1)
  AND name <> capital;
```
- **13. SELECT from world **
```
solution:
SELECT name
FROM world
WHERE name LIKE '%a%' 
  AND name LIKE '%e%' 
  AND name LIKE '%i%' 
  AND name LIKE '%o%' 
  AND name LIKE '%u%' 
  AND name NOT LIKE '% %';
```
# SELECT from world Quiz ####
- **1. SELECT from world Quiz **
![Captura de pantalla 2025-03-16 203911](https://github.com/user-attachments/assets/6024b2f0-da41-426e-b0e0-876afabcff13)
- **2. SELECT from world Quiz **
![Captura de pantalla 2025-03-16 204627](https://github.com/user-attachments/assets/7af0cf0e-74a4-46ff-a263-83d6139ee471)
- **3. SELECT from world Quiz **
![Captura de pantalla 2025-03-16 204641](https://github.com/user-attachments/assets/26b009e8-d83a-4bfd-a0ca-8685cd0407bf)
- **4. SELECT from world Quiz **
![Captura de pantalla 2025-03-16 204656](https://github.com/user-attachments/assets/196aef57-86e3-4e51-932f-a482f6c03a09)
- **5. SELECT from world Quiz **
![Captura de pantalla 2025-03-16 204710](https://github.com/user-attachments/assets/6054ad46-8a0a-4478-98fd-66fced584998)
- **6. SELECT from world Quiz **
![Captura de pantalla 2025-03-16 204725](https://github.com/user-attachments/assets/4934d82b-d933-4b05-a6ab-c7f6de969d22)
- **7. SELECT from world Quiz **
![Captura de pantalla 2025-03-16 204739](https://github.com/user-attachments/assets/d2f6080a-5dce-4d9f-80c2-1a74e2b65eb8)

# SELECT from nobel ####
- **1. SELECT from nobel **
```
Solution:
SELECT yr, subject, winner
  FROM nobel
 WHERE yr = 1950
```
- **2. SELECT from nobel **
```
Solution:
SELECT winner
FROM nobel
WHERE yr = 1962
  AND subject = 'literature';
```
- **3. SELECT from nobel **
```
Solution:
SELECT yr, subject
FROM nobel
WHERE winner = 'Albert Einstein';
```
- **4. SELECT from nobel **
```
Solution:
SELECT winner
FROM nobel
WHERE subject = 'peace'
  AND yr >= 2000;
```
- **5. SELECT from nobel **
```
Solution:
SELECT yr, subject, winner
FROM nobel
WHERE subject = 'literature'
  AND yr BETWEEN 1980 AND 1989;
```
- **6. SELECT from nobel **
```
Solution:
SELECT *
FROM nobel
WHERE winner IN ('Theodore Roosevelt',
'Thomas Woodrow Wilson', 'Jimmy Carter',
'Barack Obama');
```
- **7. SELECT from nobel **
```
Solution:
SELECT winner
FROM nobel
WHERE winner LIKE 'john%'
```
- **8. SELECT from nobel **
```
Solution:
SELECT yr, subject, winner
FROM nobel
WHERE subject = 'physics' AND yr = 1980

UNION

SELECT yr, subject, winner
FROM nobel
WHERE subject = 'chemistry' AND yr = 1984;
```
- **9. SELECT from nobel **
```
Solution:
SELECT yr, subject, winner
FROM nobel
WHERE yr = 1980
  AND subject NOT IN ('chemistry', 'medicine');
```
- **10. SELECT from nobel **
```
Solution:
SELECT yr, subject, winner
FROM nobel
WHERE subject = 'medicine' 
  AND yr < 1910

UNION

SELECT yr, subject, winner
FROM nobel
WHERE subject = 'literature' 
  AND yr >= 2004;
```
- **11. SELECT from nobel **
```
Solution:
SELECT *
FROM nobel
WHERE winner = 'PETER GRÜNBERG';
```
- **12. SELECT from nobel **
```
Solution:
SELECT *
FROM nobel
WHERE winner = 'EUGENE O''NEILL';
```
- **13. SELECT from nobel **
```
Solution:
SELECT winner, yr, subject
FROM nobel
WHERE winner LIKE 'Sir%'
ORDER BY yr DESC, winner ASC
```
- **14. SELECT from nobel **
```
Solution:
SELECT winner, subject
 FROM nobel
WHERE yr=1984
ORDER BY subject IN ('physics', 'chemistry'),subject,winner
```
# SELECT from nobel Quiz ####
- **1. SELECT from nobel Quiz **
![image](https://github.com/user-attachments/assets/8cde79a3-0b69-4cf0-ab7e-ce331986530c)
- **2. SELECT from nobel Quiz **
![image](https://github.com/user-attachments/assets/3f2ce820-4774-46b7-aad4-307890b27ce5)
- **3. SELECT from nobel Quiz **
![image](https://github.com/user-attachments/assets/c8d33476-6bde-4e62-9883-3133f4a7dad6)
- **4. SELECT from nobel Quiz **
![image](https://github.com/user-attachments/assets/c67ac6e2-7268-4a91-87ef-20305cbdb498)
- **5. SELECT from nobel Quiz **
![image](https://github.com/user-attachments/assets/2e182ba2-57d6-43bc-965d-8f367477abe9)
- **6. SELECT from nobel Quiz **
![image](https://github.com/user-attachments/assets/a35794c8-0be8-4946-b326-6b2fa806ddfb)
- **7. SELECT from nobel Quiz **
![image](https://github.com/user-attachments/assets/deb48a5f-3873-4511-8db9-d5efce476941)
# SELECT in SELECT ####
- **1. SELECT in SELECT **
```
Solution:
SELECT name
FROM world
WHERE population > (SELECT population FROM world WHERE name = 'Russia');
```
- **2. SELECT in SELECT **
```
Solution:
SELECT name
FROM world
WHERE continent = 'Europe'
  AND (gdp / population) > (SELECT gdp / population FROM world WHERE name = 'United Kingdom');
```
- **3. SELECT in SELECT **
```
Solution:
SELECT name, continent
FROM world
WHERE continent IN (
    SELECT continent
    FROM world
    WHERE name IN ('Argentina', 'Australia')
)
ORDER BY name;
```
- **4. SELECT in SELECT **
```
Solution:
SELECT name, population
FROM world
WHERE population > (SELECT population FROM world WHERE name = 'United Kingdom')
  AND population < (SELECT population FROM world WHERE name = 'Germany');
```
- **5. SELECT in SELECT **
```
Solution:
SELECT name, 
       CONCAT(ROUND((population / (SELECT population FROM world WHERE name = 'Germany')) * 100, 0), '%') AS percentage
FROM world
WHERE continent = 'Europe';
```
- **6. SELECT in SELECT **
```
Solution:
SELECT name
FROM world
WHERE gdp > (SELECT MAX(gdp) FROM world WHERE continent = 'Europe')
  AND gdp IS NOT NULL;
```
- **7. SELECT in SELECT **
```
Solution:
SELECT continent, name, area
FROM world x
WHERE area >= ALL
  (SELECT area FROM world y
   WHERE y.continent = x.continent
     AND area > 0);
```
- **8. SELECT in SELECT **
```
Solution:
SELECT continent, name
FROM world
WHERE (continent, name) IN (
    SELECT continent, MIN(name)
    FROM world
    GROUP BY continent
);
```
- **9. SELECT in SELECT **
```
Solution:
SELECT name, continent, population
FROM world
WHERE continent IN (
    SELECT continent
    FROM world
    GROUP BY continent
    HAVING MAX(population) <= 25000000
);
```
- **10. SELECT in SELECT **
```
Solution:
SELECT name, continent
FROM world x
WHERE population/3 > ALL(
SELECT population
FROM world y
WHERE x.continent = y.continent
AND x.name != y.name)
```
# SELECT in SELECT Quiz ####
- **1. SELECT in SELECT Quiz **
![image](https://github.com/user-attachments/assets/d13d2413-04da-4385-9ec3-515cca0b550e)
- **2. SELECT in SELECT Quiz **
![image](https://github.com/user-attachments/assets/3e6c903b-cd0e-4514-85bb-da53fd025511)
- **3. SELECT in SELECT Quiz **
![image](https://github.com/user-attachments/assets/e0721d98-06de-4477-af60-17929b1f4494)
- **4. SELECT in SELECT Quiz **
![image](https://github.com/user-attachments/assets/513dc6b3-5b80-4508-a62e-d20e180360e1)
- **5. SELECT in SELECT Quiz **
![image](https://github.com/user-attachments/assets/81b419fa-d0c1-410b-8cda-2361b862f1a2)
- **6. SELECT in SELECT Quiz **
![image](https://github.com/user-attachments/assets/0efdf05a-8956-464b-8d34-778c91307b1e)
- **7. SELECT in SELECT Quiz **
![image](https://github.com/user-attachments/assets/8bbb7bf3-14d6-409f-ab47-77b6956c1e31)
# SUM and COUNT ####
- **1. SUM and COUNT **
```
Solution:
SELECT SUM(population)
FROM world
```
- **2. SUM and COUNT **
```
Solution:
SELECT DISTINCT continent
FROM world;
```
- **3. SUM and COUNT **
```
Solution:
SELECT SUM(gdp) AS total_gdp
FROM world
WHERE continent = 'Africa';
```
- **4. SUM and COUNT **
```
Solution:
SELECT COUNT(*)
FROM world
WHERE area >= 1000000;
```
- **5. SUM and COUNT **
```
Solution:
SELECT SUM(population)
FROM world
WHERE name IN ('Estonia', 'Latvia', 'Lithuania');
```
- **6. SUM and COUNT **
```
Solution:
SELECT continent, COUNT(name) AS num_countries
FROM world
GROUP BY continent;
```
- **7. SUM and COUNT **
```
Solution:
SELECT continent, COUNT(name) AS num_countries
FROM world
WHERE population >= 10000000
GROUP BY continent;
```
- **8. SUM and COUNT **
```
Solution:
SELECT continent
FROM world
GROUP BY continent
HAVING SUM(population) >= 100000000;
```
# SUM and COUNT Quiz ####
- **1. SUM and COUNT Quiz **
![image](https://github.com/user-attachments/assets/722cd369-e271-4600-80bc-2bf9173217db)
- **2. SUM and COUNT Quiz **
![image](https://github.com/user-attachments/assets/0baa0ab6-cdd8-4d20-bcd3-78f5bfda723a)
- **3. SUM and COUNT Quiz **
![image](https://github.com/user-attachments/assets/55f3a35e-494f-4919-8d13-f89c34e8160b)
- **4. SUM and COUNT Quiz **
![image](https://github.com/user-attachments/assets/a72f263f-3cdc-4147-8bc0-237bb2cef7b8)d
- **5. SUM and COUNT Quiz **
![image](https://github.com/user-attachments/assets/e5a772e4-5d37-4818-b7b1-4062d2411d11)
- **6. SUM and COUNT Quiz **
![image](https://github.com/user-attachments/assets/021e7105-3c16-4edb-bf72-1e183f1d11f9)
- **7. SUM and COUNT Quiz **
![image](https://github.com/user-attachments/assets/788f03e5-ddc2-4eb6-8473-74966554f42e)
- **8. SUM and COUNT Quiz **
![image](https://github.com/user-attachments/assets/48fad411-e8ba-4f6e-a64c-6959cb1c2b90)
# JOIN ####
- **1. JOIN **
```
Solution:
SELECT matchid, player 
FROM goal 
WHERE teamid = 'GER';
```
- **2. JOIN **
```
Solution:
SELECT id, stadium, team1, team2
FROM game
WHERE id = 1012;
```
- **3. JOIN **
```
Solution:
SELECT player, teamid, stadium, mdate
FROM game
JOIN goal ON game.id = goal.matchid
WHERE teamid = 'GER';
```
- **4. JOIN **
```
Solution:
SELECT team1, team2, player
FROM game
JOIN goal ON game.id = goal.matchid
WHERE player LIKE 'Mario%';
```
- **5. JOIN **
```
Solution:
SELECT player, teamid, coach, gtime
FROM goal
JOIN eteam ON goal.teamid = eteam.id
WHERE gtime <= 10;
```
- **6. JOIN **
```
Solution:
select mdate, teamname from game JOIN eteam ON
(team1=eteam.id) where coach = 'Fernando Santos'
```
- **7. JOIN **
```
Solution:
SELECT goal.player
FROM game
JOIN goal ON game.id = goal.matchid
WHERE game.stadium = 'National Stadium, Warsaw';
```
- **8. JOIN **
```
Solution:
SELECT distinct player
FROM game JOIN goal ON matchid = id 
WHERE (team1='GER' OR team2='GER') AND teamid <> 'GER'
```
- **9. JOIN **
```
Solution:
SELECT teamname, COUNT(*)
FROM eteam JOIN goal ON id=teamid
GROUP BY teamname;
```
- **10. JOIN **
```
Solution:
SELECT stadium, COUNT(*) AS total_goals
FROM game
JOIN goal ON game.id = goal.matchid
GROUP BY stadium;
```
- **11. JOIN **
```
Solution:
SELECT game.id AS matchid, game.mdate AS date, COUNT(goal.matchid) AS total_goals
FROM game
JOIN goal ON game.id = goal.matchid
WHERE game.team1 = 'POL' OR game.team2 = 'POL'
GROUP BY game.id, game.mdate;
```
- **12. JOIN **
```
Solution:
SELECT game.id AS matchid, game.mdate AS date, COUNT(goal.matchid) AS goals_scored_by_GER
FROM game
JOIN goal ON game.id = goal.matchid
WHERE (game.team1 = 'GER' AND goal.teamid = 'GER') 
   OR (game.team2 = 'GER' AND goal.teamid = 'GER')
GROUP BY game.id, game.mdate;
```
- **13. JOIN **
```
Solution:
SELECT mdate,
  team1, sum(CASE WHEN teamid=team1 THEN 1 ELSE 0 END) score1, team2,sum(CASE WHEN teamid=team2 THEN 1 ELSE 0 END) score2
  FROM game JOIN goal ON matchid = id
GROUP BY mdate,matchid,team1,team2
order by mdate, matchid, team1, team2
```
# JOIN Quiz ####
- **1. JOIN Quiz **
![image](https://github.com/user-attachments/assets/f07a4e00-a58f-40fe-83b8-23ce422c9279)
- **1. JOIN Quiz **
![image](https://github.com/user-attachments/assets/c9708167-d280-40e1-8e88-a84ed2bcc30f)
- **1. JOIN Quiz **
![image](https://github.com/user-attachments/assets/3d119635-8b1a-4f1c-b4dd-6e99acc88cf8)
- **1. JOIN Quiz **
![image](https://github.com/user-attachments/assets/6c1e5db9-a81a-4f77-94dd-66c03811c6ed)
- **1. JOIN Quiz **
![image](https://github.com/user-attachments/assets/c163b8ef-a027-4d71-a1b9-d4e410ac0143)
- **1. JOIN Quiz **
![image](https://github.com/user-attachments/assets/dadcaef9-3d0f-47d5-b907-3c8250a2a423)
- **1. JOIN Quiz **
![image](https://github.com/user-attachments/assets/5f209c3a-a869-4022-9e3d-d955fb353ee5)
# More JOIN ####
- **1. More JOIN **
```
Solution:
SELECT id, title
 FROM movie
 WHERE yr=1962
```
- **2. More JOIN **
```
Solution:
SELECT yr
FROM movie
WHERE title='Citizen Kane'
```
- **3. More JOIN **
```
Solution:
SELECT id, title, yr
FROM movie
WHERE title LIKE '%Star Trek%'
ORDER BY yr;
```
- **4. More JOIN **
```
Solution:
SELECT id
FROM actor
WHERE name = 'Glenn Close';
```
- **5. More JOIN **
```
Solution:
SELECT id
FROM movie
WHERE title = 'Casablanca'
```
- **6. More JOIN **
```
Solution:
SELECT actor.name
FROM actor
JOIN casting ON actor.id = casting.actorid
WHERE casting.movieid = 11768;
```
- **7. More JOIN **
```
Solution:
SELECT actor.name
FROM actor
JOIN casting ON actor.id = casting.actorid
JOIN movie ON casting.movieid = movie.id
WHERE movie.title = 'Alien';

```
- **8. More JOIN **
```
Solution:
SELECT movie.title
FROM movie
JOIN casting ON movie.id = casting.movieid
JOIN actor ON actor.id = casting.actorid
WHERE actor.name = 'Harrison Ford';
```
- **9. More JOIN **
```
Solution:
SELECT movie.title
FROM movie
JOIN casting ON movie.id = casting.movieid
JOIN actor ON actor.id = casting.actorid
WHERE actor.name = 'Harrison Ford'
  AND casting.ord != 1;
```
- **10. More JOIN **
```
Solution:

```
- **11. More JOIN **
```
Solution:

```
- **12. More JOIN **
```
Solution:
SELECT m.title, a.name AS leading_actor
FROM movie m
JOIN casting c ON m.id = c.movieid
JOIN actor a ON c.actorid = a.id
WHERE c.ord = 1
  AND m.id IN (
      SELECT m.id
      FROM movie m
      JOIN casting c ON m.id = c.movieid
      JOIN actor a ON c.actorid = a.id
      WHERE a.name = 'Julie Andrews'
  )
ORDER BY m.title;
```
- **13. More JOIN **
```
Solution:
SELECT a.name
FROM actor a
JOIN casting c ON a.id = c.actorid
WHERE c.ord = 1  -- This ensures the actor is in the starring role
GROUP BY a.name
HAVING COUNT(c.movieid) >= 15
ORDER BY a.name;
```
- **14. More JOIN **
```
Solution:
SELECT m.title, COUNT(c.actorid) AS actor_count
FROM movie m
JOIN casting c ON m.id = c.movieid
WHERE m.yr = 1978
GROUP BY m.title
ORDER BY actor_count DESC, m.title;
```
- **15. More JOIN **
```
Solution:
SELECT DISTINCT a.name
FROM actor a
JOIN casting c ON a.id = c.actorid
JOIN movie m ON c.movieid = m.id
WHERE m.id IN (
    SELECT movieid
    FROM casting
    JOIN actor ON casting.actorid = actor.id
    WHERE actor.name = 'Art Garfunkel'
)
AND a.name != 'Art Garfunkel';
```
# More JOIN Quiz ####
- **1. More JOIN Quiz **
![image](https://github.com/user-attachments/assets/19f4c914-fccf-4dfc-b486-ed6c2ebd35ee)
- **2. More JOIN Quiz **
![image](https://github.com/user-attachments/assets/3c249118-b237-4f32-953a-0c6752181039)
- **3. More JOIN Quiz **
![image](https://github.com/user-attachments/assets/f6455954-daf1-405e-9824-f9d211be0fcb)
- **4. More JOIN Quiz **
![image](https://github.com/user-attachments/assets/b7d186f6-4842-4091-9d33-6e83a64c29ea)
- **5. More JOIN Quiz **
![image](https://github.com/user-attachments/assets/ceafacc0-28f8-47ec-ab48-7ca9f63e1933)
- **6. More JOIN Quiz **
![image](https://github.com/user-attachments/assets/49d4424d-e40a-4065-88fa-55a0d1a27536)
- **7. More JOIN Quiz **
![image](https://github.com/user-attachments/assets/40c08574-94f9-4d06-a9bd-d80c81ab5a88)
# Using NULL ####
- **1. Using NULL **
```
Solution:
SELECT name
FROM teacher
WHERE dept IS NULL;
```
- **2. Using NULL **
```
Solution:
SELECT teacher.name, dept.name
 FROM teacher INNER JOIN dept
           ON (teacher.dept=dept.id)
```
- **3. Using NULL **
```
Solution:
SELECT teacher.name, dept.name 
FROM teacher 
LEFT JOIN dept 
 ON (teacher.dept=dept.id)
```
- **4. Using NULL **
```
Solution:
SELECT teacher.name, dept.name 
FROM teacher 
RIGHT JOIN dept 
 ON (teacher.dept=dept.id)
```
- **5. Using NULL **
```
Solution:
SELECT name, COALESCE(mobile, '07986 444 2266') 
FROM teacher;
```
- **6. Using NULL **
```
Solution:
SELECT teacher.name, COALESCE(dept.name, 'None')
FROM teacher
LEFT JOIN dept 
 ON (teacher.dept=dept.id)
```
- **7. Using NULL **
```
Solution:
SELECT 
    COUNT(teacher.id) AS number_of_teachers,
    COUNT(teacher.mobile) AS number_of_mobile_phones
FROM teacher;
```
- **8. Using NULL **
```
Solution:
SELECT dept.name, COUNT(teacher.name) 
FROM teacher
RIGHT JOIN dept
    ON (teacher.dept=dept.id)
GROUP BY dept.name;
```
- **9. Using NULL **
```
Solution:
SELECT name, 
CASE WHEN teacher.dept = 1 OR teacher.dept = 2 THEN 'Sci' ELSE 'Art' END
FROM teacher
```
- **10. Using NULL **
```
Solution:
SELECT name, 
CASE 
WHEN teacher.dept = 1 OR teacher.dept = 2 THEN 'Sci'
WHEN teacher.dept = 3 THEN'Art'
ELSE 'None'END
FROM teacher
```
# Using NULL Quiz ####
- **1. Using NULL Quiz **
![image](https://github.com/user-attachments/assets/3917ac1f-d436-4413-982b-7881602324e7)
- **2. Using NULL Quiz **
![image](https://github.com/user-attachments/assets/d694e165-45cb-4ce6-9c8e-003a2c63f9a1)
- **3. Using NULL Quiz **
![image](https://github.com/user-attachments/assets/55fb3890-8011-4bd8-a273-7ee2d131fab1)
- **4. Using NULL Quiz **
![image](https://github.com/user-attachments/assets/20b87f44-5012-4e95-8f09-c25ac7f8aae1)
- **5. Using NULL Quiz **
![image](https://github.com/user-attachments/assets/f3665b91-0b55-4416-9541-9a0e0b627070)
- **6. Using NULL Quiz **
![image](https://github.com/user-attachments/assets/3a5097c8-7bb4-4e73-8fa8-49c5f1ff1474)
# self JOIN ####
- **1. self JOIN **
```
Solution:
SELECT COUNT(*) 
FROM stops
```
- **2. self JOIN **
```
Solution:
SELECT id
FROM stops
WHERE name = 'Craiglockhart'
```
- **3. self JOIN **
```
Solution:
SELECT stops.id, stops.name
FROM stops
JOIN route ON stops.id = route.stop
WHERE route.num = '4' AND route.company = 'LRT';
```
- **4. self JOIN **
```
Solution:
SELECT company, num, COUNT(*)
FROM route
WHERE stop = 149 OR stop = 53
GROUP BY company, num
HAVING COUNT(*) = 2;
```
- **5. self JOIN **
```
Solution:
SELECT a.company, a.num, a.stop, b.stop
FROM route a
JOIN route b ON (a.company = b.company AND a.num = b.num)
WHERE a.stop = 53 AND b.stop = 149;
```
- **6. self JOIN **
```
Solution:
SELECT a.company, a.num, stopa.name, stopb.name
FROM route a
JOIN route b ON (a.company = b.company AND a.num = b.num)
JOIN stops stopa ON (a.stop = stopa.id)
JOIN stops stopb ON (b.stop = stopb.id)
WHERE stopa.name = 'Craiglockhart' AND stopb.name = 'London Road';
```
- **7. self JOIN **
```
Solution:
SELECT DISTINCT a.company,a.num
FROM route a JOIN route b ON 
(a.company=b.company AND a.num=b.num)
JOIN stops stopa ON(a.stop=stopa.id)
JOIN stops stopb ON(b.stop=stopb.id)
WHERE stopa.name='Haymarket' AND stopb.name= 'Leith'
```
- **8. self JOIN **
```
Solution:
SELECT a.company, a.num
FROM route a
JOIN route b ON (a.company = b.company AND a.num = b.num)
JOIN stops stopa ON (a.stop = stopa.id)
JOIN stops stopb ON (b.stop = stopb.id)
WHERE stopa.name = 'Craiglockhart' AND stopb.name = 'Tollcross';
```
- **9. self JOIN **
```
Solution:
SELECT DISTINCT stopb.name,a.company,a.num
FROM route a JOIN route b ON 
(a.company=b.company AND a.num=b.num)
JOIN stops stopa ON(a.stop=stopa.id)
JOIN stops stopb ON(b.stop=stopb.id)
WHERE stopa.name='Craiglockhart' 
AND a.company='LRT'
```
# self JOIN Quiz ####
- **1. self JOIN Quiz  **
![image](https://github.com/user-attachments/assets/683e58fa-c70f-4301-8bbd-4bfc55a87313)
- **2. self JOIN Quiz  **
![image](https://github.com/user-attachments/assets/638cda12-f3b2-48df-ba31-7c4a5224c219)
- **3. self JOIN Quiz  **
![image](https://github.com/user-attachments/assets/82e7a425-4145-4215-a24b-d14676c15a0f)



