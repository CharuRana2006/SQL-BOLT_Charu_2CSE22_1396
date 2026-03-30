# SQL LAB-BOLT EXERCISE-4

## 1. List all directors of Pixar movies (alphabetically), without duplicates.
```sql
SELECT DISTINCT director FROM movies ORDER BY director ASC;
```
# Output
| director         |
|------------------|
| Andrew Stanton   |
| Brad Bird        |
| Brenda Chapman   |
| Dan Scanlon      |
| John Lasseter    |
| Lee Unkrich      |
| Pete Docter      |

## 2. List the last four Pixar movies released (ordered from most recent to least) .
```sql
SELECT * FROM movies ORDER BY year DESC LIMIT 4;
```
# Output
| id | title              | director        | year | length_minutes |
|----|--------------------|-----------------|------|----------------|
| 4  | Monsters University| Dan Scanlon     | 2013 | 110            |
| 8  | Brave              | Brenda Chapman  | 2012 | 102            |
| 12 | Cars 2             | John Lasseter   | 2011 | 120            |
| 1  | Toy Story 3        | Lee Unkrich     | 2010 | 103            |

## 3. List the first five Pixar movies sorted alphabetically .
```sql
SELECT * FROM movies ORDER BY title ASC LIMIT 5;
```
# Output
| id | title         | director        | year | length_minutes |
|----|---------------|-----------------|------|----------------|
| 5  | A Bug's Life  | John Lasseter   | 1998 | 95             |
| 8  | Brave         | Brenda Chapman  | 2012 | 102            |
| 11 | Cars          | John Lasseter   | 2006 | 117            |
| 12 | Cars 2        | John Lasseter   | 2011 | 120            |
| 9  | Finding Nemo  | Andrew Stanton  | 2003 | 107            |

## 4. List the next five Pixar movies sorted alphabetically .
```sql
SELECT * FROM movies ORDER BY title ASC LIMIT 5 OFFSET 5;
```
# Output
| id | title              | director        | year | length_minutes |
|----|--------------------|-----------------|------|----------------|
| 14 | Monsters, Inc.     | Pete Docter     | 2001 | 92             |
| 4  | Monsters University| Dan Scanlon     | 2013 | 110            |
| 2  | Ratatouille        | Brad Bird       | 2007 | 115            |
| 3  | The Incredibles    | Brad Bird       | 2004 | 116            |
| 13 | Toy Story          | John Lasseter   | 1995 | 81             |