Lab 03: SQL injection attack, querying the database type and version on Oracle
![before_solve](image/lap03before.png)

 Use Burp Suite to intercept and modify the request that sets the product category filter.
Determine the number of columns that are being returned by the query and which columns contain text data. Verify that the query is returning two columns, both of which contain text, using a payload like the following in the category parameter:
'+UNION+SELECT+'abc','def'+FROM+dual--
Use the following payload to display the database version:
'+UNION+SELECT+BANNER,+NULL+FROM+v$version--
![proses-to-solve-this-lab](image/proses03.png)
![this-lab-is-solved](image/lab03solved.png)
