---
tags:
  - queries
  - sql
---
Oscar Lopez
CS 443
[[2024-10-21]]

# queries 
____
* Queries most important thing sql can do.
* Queries let you retrieve relevant data from other tables. 
  * The flexibility of SQL will be seen as we progress in the course.

## Constraint
___
- Consider the following table creations
```sql
CREATE TABLE Employee
(
 Emp NUMBER(6) PRIMARY KEY,
 FirstName VARCHAR(10) NOT NULL,
 LastName VARCHAR(12) NOT NULL,
 DeptNo VARCHAR(12),
 HireDate DATE NOT NULL
);
```
## Insert
___
- The INSERT SQL command is used to insert rows of data into a table.

```sql
INSERT INTO Employee
	VALUES(1001,'Ben','Li','Mathematics','21-APR-89');
```

## Select
___
- The SELECT statement is one of the most basic statements one can use in SQL. In its most basic form, its very simple to use.

- Suppose we have the following table.


| City          | Target     | Sales      |
| ------------- | ---------- | ---------- |
| Winnipeg      | $50,000.00 | $23,123.00 |
| Brandon       | $4,000.00  | $4,500.00  |
| Selkirk       | $2,000.00  | $1,200.00  |
| Beausejour    | $1000.00   | $235.00    |
| Lac du Bonnet | $500.00    | $345.00    |
Question:
	List all cities, target sales and sales
Query:
	```sql
		SELECT City, Target, Sales
		 FROM Cities
	```
Result:

| City          | Target     | Sales      |
| ------------- | ---------- | ---------- |
| Beausejour    | $1,000.00  | $235.00    |
| Brandon       | $4,000.00  | $4,500.00  |
| Lac de Bonnet | $500.00    | $345.00    |
| Selkirk       | $2,000.00  | $1,200.00  |
| Winnipeg      | $50,000.00 | $23,123.00 |


# Equi-Joins
___


	
