# SQL LAB-BOLT EXERCISE-5

## 1. List all the Canadian cities and their populations.
```sql
SELECT city, population FROM north_american_cities WHERE country = 'Canada';
```
# Output
| city     | population |
|----------|------------|
| Toronto  | 2795060    |
| Montreal | 1717767    |

## 2. Order all the cities in the United States by their latitude from north to south.
```sql
SELECT city, latitude FROM north_american_cities WHERE country = 'United States' ORDER BY latitude DESC;
```
# Output
| city        | latitude  |
|-------------|-----------|
| Chicago     | 41.878114 |
| New York    | 40.712784 |
| Philadelphia| 39.952584 |
| Los Angeles | 34.052234 |
| Phoenix     | 33.448377 |
| Houston     | 29.760427 |

## 3. List all the cities west of Chicago, ordered from west to east.
```sql
SELECT city, longitude FROM north_american_cities WHERE longitude < -87.629798 ORDER BY longitude ASC;
```
# Output
| city                | longitude   |
|---------------------|-------------|
| Los Angeles         | -118.243685 |
| Phoenix             | -112.074037 |
| Guadalajara         | -103.349609 |
| Mexico City         | -99.133208  |
| Ecatepec de Morelos | -99.050674  |
| Houston             | -95.369803  |

## 4. List the two largest cities in Mexico (by population).
```sql
SELECT city, population FROM north_american_cities WHERE country = 'Mexico' ORDER BY population DESC LIMIT 2;
```
# Output
| city        | population |
|-------------|------------|
| Mexico City | 8555500    |
| Ecatepec de Morelos | 1742000 |

## 5. List the third and fourth largest cities (by population) in the United States and their population.
```sql
SELECT city, population FROM north_american_cities WHERE country = 'United States' ORDER BY population DESC LIMIT 2 OFFSET 2;
```
# Output
| city      | population |
|-----------|------------|
| Chicago   | 2718782    |
| Houston   | 2195914    |