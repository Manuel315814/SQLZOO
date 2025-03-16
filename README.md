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
SELECT name, continent, population FROM world
```
- **1. SELECT from world **
```
solution:
SELECT name, continent, population FROM world
```
- **1. SELECT from world **
```
solution:
SELECT name, continent, population FROM world
```
- **1. SELECT from world **
```
solution:
SELECT name, continent, population FROM world
```
- **1. SELECT from world **
```
SELECT name, continent, population FROM world
```
- **1. SELECT from world **
```
SELECT name, continent, population FROM world
```
