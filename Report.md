# DSM23 Project Phase - 2

Submission date: 

Submitted By
| Roll number | Names |
|-----------|-----------|
| 2022201004 | Yash Singhal |
| 2022201079 | Priyanshu Bansal |
| 2022202023 | Anurag Ghosh |

## Assumptions
<ul>
  <li> </li>
  <li> </li>
</ul>

## External Sort
#### Syntax
```sql
SORT <table_name> BY <column_name1, column_name2,..., column_namek> IN
<ASC|DESC, ASC|DESC,..., ASC|DESC>
```
#### Example
```sql
SORT EMPLOYEE BY GENDER, SALARY IN ASC, DESC
```

## JOIN
#### Syntax
```sql
<new_relation_name> <- JOIN <tablename1>, <tablename2> ON <column1>
<bin_op> <column2>
```
#### Example
```sql
Result <- JOIN Students, Courses ON ID == RollNo 
```

## Order By
#### Syntax
```sql
<new_table> <- ORDER BY <attribute> ASC|DESC ON <table_name>
```
#### Example
```sql
Result <- ORDER BY Year_Released ASC ON Movies
```

## Group By
#### Syntax
```sql
<new_table> <- GROUP BY <grouping_attribute> FROM <table_name> HAVING
<aggregate(attribute)> <bin_op> <attribute_value> RETURN
<aggregate_func(attribute)>
```
#### Example
```sql
T1 <- GROUP BY Department_ID FROM EMPLOYEE HAVING
AVG(Salary) > 50,000 RETURN MAX(Salary)
```
