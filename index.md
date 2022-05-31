**Name**: Usha Gunale  

**Date**: May 30, 2022  

**Course**: IT FDN 130 A Spring 22 

**Assignment 07**: FUNCTIONS
**GitHub Url**:https://github.com/UGunale2/DBFoundations-Module07
 

# FUNCTION

**Introduction**: In this module, I discuss when you would use a SQL UDF, the differences between Scalar, Inline, and Multi-Statement, and use Professor Randal Root’s material to prepare this document.

## EXPLAIN WHEN YOU WOULD USE A SQL UDF. 

SQL UDFs are a powerful tool, and when the database has the repeatedly same logic multiple times, you can create the SQL UDF once, and wherever needed, that function calls it. SQL UDFs reduce the client/server network traffic. You can reuse them. 
## EXPLAIN ARE THE DIFFERENCES BETWEEN SCALAR, INLINE, AND MULTI-STATEMENT FUNCTIONS.

### SCALAR FUNCTION :

Scalar functions may or may not take input parameters and return a single value result. The returned value can be of any data type, except text, ntext, image, cursor, and timestamp.

## SYNTAX FOR CREATING A SCALAR FUNCTION

```sql
CREATE FUNCTION [schema_name.]function_name (parameter_list)
returns data_type AS
BEGIN
  statements
  RETURN value
ENd 
```
### INLINE FUNCTION :

A table function is invoked in the FROM clause of a SELECT statement and returns a table to the statement.

## SYNTAX FOR CREATING A INLINE FUNCTION

```sql
CREATE FUNCTION function_name(@Param1 DATATYPE,
@Param2 datatype...,
@ParamN datatype)
returns TABLE AS
RETURN (select_statement) 
```
### MUTLTI-STATEMENT FUNCTION:

Multi statement table valued functions are very similar to Inline Table valued functions.
A multi-statement table-valued function is a function which returns a table of data, but only after some additional processing.

## DIFFERENCES BETWEEN THEM:

1.In an Inline Table Valued function, the RETURNS clause cannot contain the structure of the table, the function returns. Where as, with the multi-statement table valued function, we specify the structure of the table that gets returned

2. Inline Table Valued function cannot have BEGIN and END block, where as the multi-statement function can have.

3. Inline Table valued functions are better for performance, than multi-statement table valued functions. If the given task, can be achieved using an inline table valued function, always prefer to use them, over multi-statement table valued functions.

4. It's possible to update the underlying table, using an inline table valued function, but not possible using multi-statement table valued function

## Summary

This article learns about when you would use a SQL Functions, and the differences between a Scalar, Inline and Multi-Statement Functions.
### GitHub Links:
Assignment07_UGunale.Sql Script and Assignment07_UGunale.PDF file : https://github.com/UGunale2/DBFoundations-Module07
GitHub Webpage : https://github.com/UGunale2/DBFoundations-Module07/blob/main/index.md
### Image link :
![This is an image](https://myoctocat.com/assets/images/base-octocat.svg)






