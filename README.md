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
```
![image](https://github.com/user-attachments/assets/b624ae24-da0a-43c2-accb-63e98af80f40)
```
- **2. SELECT basics Quiz **
```
![image](https://github.com/user-attachments/assets/52cc38b6-bf1d-4a66-92ee-c8bab8ac4368)
```
- **3. SELECT basics Quiz **
```
![image](https://github.com/user-attachments/assets/de8df29b-7ddc-48e8-a3e4-4eecb6a100cb)
```
- **4. SELECT basics Quiz **
```
![image](https://github.com/user-attachments/assets/cdcb9fd6-582a-468a-aa4c-df327447770a)
```
- **5. SELECT basics Quiz **
```
![image](https://github.com/user-attachments/assets/bdf9465b-fa07-4a77-ab80-6ea49ab1a7e5)
```
- **6. SELECT basics Quiz **
```
![image](https://github.com/user-attachments/assets/8303f2ff-ae0c-4cc8-a0b4-a262c1402096)
```
- **7. SELECT basics Quiz **
```
![image](https://github.com/user-attachments/assets/aa4c2d2b-633c-49a6-b7cc-c808d5366097)
```
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

