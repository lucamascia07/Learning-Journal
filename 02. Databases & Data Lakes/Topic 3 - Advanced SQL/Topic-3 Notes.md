# Topic 3 - Advanced SQL

## What is a EQUI join?
EQUI JOIN is a simple SQL join and uses the equal sign(=) as  the comparison operator for the condition

## What is a NON EQUI join?
NON EQUI JOIN  uses comparison operator other than the equal sign the operators uses  like >, <, >=, <= with the condition.

## What is a Inner Join?
Returns only matched rows from the participating tables and a match happened only at the key record of participating tables. The INNER JOIN selects all rows from both participating tables as long as there is a match between the columns. An SQL INNER JOIN is same as JOIN clause, combining rows from two or more tables.

## What is a Left Join?
The SQL LEFT JOIN, joins two tables and fetches rows based on a condition, which are matching in both the tables and the unmatched rows will also be available from the RIGHT table before the JOIN clause.

## What is a Right Join?
The SQL RIGHT JOIN, joins two tables and fetches rows based on a condition, which are matching in both the tables and the unmatched rows will also be available from the LEFT table written after the JOIN clause.

## What is a Cross Join?
The SQL CROSS JOIN produces a result set which is the number of rows in the first table multiplied by the number of rows in the second table, if no WHERE clause is used along with CROSS JOIN. This kind of result is called as Cartesian Product. If, WHERE clause is used with CROSS JOIN, it functions like an INNER JOIN.

## What is Union?
The UNION operator is used to combine the result-set of two or more SELECT statements. Every SELECT statement within UNION must have the same number of columns. The columns must also have similar data types and the columns in every SELECT statement must also be in the same order

## What is a Subquery?
In SQL a Subquery can be simply defined as a query within another query. In other words we can say that a Subquery is a query that is embedded in WHERE clause of another SQL query.
### Important rules for Subqueries: 
1. You can place the Subquery in a number of SQL clauses: WHERE FROM clause. clause, HAVING
2. Subqueries can be used with SELECT, UPDATE, INSERT, DELETE statements along with expression operator. It could be equality operator or comparison operator such as =, >, =, <= and Like operator. clause
3. The subquery generally executes first, and its output is used to complete the query condition for the main or outer query.
4. Subquery must be enclosed in parentheses.


## Understanding WHERE, GROUP BY and HAVING

These three SQL clauses work together but perform different jobs.

### Order of operation

**1. WHERE – Filters individual rows**
- Filters records before they are grouped.
- Used to specify conditions on individual columns.
- Example: `WHERE role = 'Engineer'`

⬇️

**2. GROUP BY – Groups rows together**
- Combines records that share the same value in a specified column.
- Commonly used with aggregate functions such as `COUNT

⬇️

3. HAVING – Filters groups

Filters the results after the groups have been created.

Particularly useful when filtering using aggregate functions.

Example: HAVING COUNT(*) > 2

Example

Find roles that have more than 2 employees:

SELECT role, COUNT(*)
FROM employees
GROUP BY role
HAVING COUNT(*) > 2;

Key differences

Clause

Purpose

WHERE

Filters individual rows

GROUP BY

Groups matching records

HAVING

Filters grouped results

Remember:

WHERE = Filter before grouping.

GROUP BY = Create groups.

HAVING = Filter after grouping.

You can also use WHERE and HAVING in the same query. WHERE first filters the individual records, GROUP BY creates the groups, and HAVING filters those groups.
