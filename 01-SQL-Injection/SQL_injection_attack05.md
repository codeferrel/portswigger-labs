Lab: SQL injection attack, listing the database contents on non-Oracle databases

End goals: <br>
determine the table that contains username and password <br>
-output the content of the table<br>
-login as a administrator user<br>
![before_solve](image/before05.png)<br>
 Use the following payload to retrieve the list of tables in the database:
'+UNION+SELECT+table_name,+NULL+FROM+information_schema.tables--<br>
![before_solve](image/proses05-1.png)<br>
Use the following payload (replacing the table name) to retrieve the details of the columns in the table: 
![before_solve](image/proses05-2.png)<br>
Use the following payload (replacing the table and column names) to retrieve the usernames and passwords for all users and get the username and password.<br>
![before_solve](image/proses05-3.png)<br>
Now we use the username and the password to login as a administrator and BOOM we solved the Lab.
![After_solved](image/solved05.png)


