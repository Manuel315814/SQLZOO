# SQLZOO

# SELECT basics ####

- **1. SELECT basics **
solution: 
SELECT population FROM world
  WHERE name = 'Germany'
- **2. SELECT basics **
solution:
SELECT name, population FROM world
  WHERE name IN ('Sweden', 'Norway', 'Denmark');
- **3. SELECT basics **
solution:
SELECT name, area FROM world
  WHERE area BETWEEN 200000 AND 250000

# SELECT names #

1
solution:
SELECT name FROM world
  WHERE name LIKE 'Y%'
2
solution:
SELECT name FROM world
  WHERE name LIKE '%Y'
3
solution:
SELECT name FROM world
  WHERE name LIKE '%x%'
4
solution:
SELECT name FROM world
  WHERE name LIKE '%land'
5
solution:
SELECT name FROM world
  WHERE name LIKE 'C%ia'
6
solution:
SELECT name FROM world
  WHERE name LIKE '%oo%'
7
solution:
SELECT name FROM world
  WHERE name LIKE '%a%a%a%'
8
solution:
SELECT name FROM world
 WHERE name LIKE '_t%'
ORDER BY name
9
solution:
SELECT name FROM world
 WHERE name LIKE '%o__o%'
10
solution:
SELECT name FROM world
 WHERE length (name)=4
## Harder Questions ##
11
solution:
SELECT name
  FROM world
 WHERE name=capital
12
solution:
SELECT name
  FROM world
 WHERE capital LIKE '% City'
13
solution:
SELECT capital, name
FROM world
WHERE
  capital LIKE CONCAT('%',name,'%')
14
solution:
SELECT capital, name
FROM world
WHERE
  capital LIKE CONCAT('%',name,'%')
AND 
   length(capital)>length(name)
