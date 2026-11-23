Lab: SQL injection UNION attack, determining the number of columns returned by the query

This lab contains a SQL injection vulnerability in the product category filter. The results from the query are returned in the application's response, so you can use a UNION attack to retrieve data from other tables. The first step of such an attack is to determine the number of columns that are being returned by the query. You will then use this technique in subsequent labs to construct the full attack.
To solve the lab, determine the number of columns returned by the query by performing a SQL injection UNION attack that returns an additional row containing null values.   

![Before solve](image/sqlb7.png)
to solve the lab used the ORDER BY technique to determine the number of columns returned by the SQL query. I tried ORDER BY 1--, ORDER BY 2--, ORDER BY 3-- until I found that 3 columns were returned. Then I used UNION SELECT NULL,NULL,NULL-- to confirm and return an additional row with NULL values. 

![after solved the lab](image/sqla7.png)