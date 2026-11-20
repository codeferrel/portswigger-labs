Lab: Basic SSRF against the local server This lab has a stock check feature which fetches data from an internal system. To solve the lab, change the stock check URL to access the admin interface at #http://localhost/admin and delete the user carlos. 
![before solve the lab](image1/ssrf1b.png)

so solve this lab change the api stochapi to stockApi=http://localhost/admin and thne delete carlos we can delete in browser or use bursuite 
![after solve this lab](image1/ssrf1p.png)
And we solved the lab
![after solve this lab](image1/ssrf1s.png)