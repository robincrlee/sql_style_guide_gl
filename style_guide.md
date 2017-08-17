## Indentation 
Clauses should be indented on the left unless it's short query. 
Some clauses are SELECT, FROM, WHERE, GROUP BY, ORDER BY, HAVING.   
Operators, such as AND, OR, IN, are not clauses. Hence, they should be at the start of a line. 

### BAD
```
SELECT col1, col2, col3  FROM table 
WHERE col1 in ('value1', 'value2')
AND col2 IS NOT NULL
```
FROM is not on the left. AND should not be at the start of a line. 

### GOOD

```
SELECT col1, col2, col3
FROM table
WHERE col1 in ('value1', 'value2') AND 
      col2 IS NOT NULL
```
Only the clauses are indented on the left. The second line in the where clause is also indented clearly. 

### also good
```
select col1, col2, col3
from table
where col1 in ('value1', 'value2') and 
      col2 is not null
```
Upper and lower cases are not that important, as long as you're consistent about them. 
