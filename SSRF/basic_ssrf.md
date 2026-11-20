Lab: Basic SSRF against the local server
This lab has a stock check feature which fetches data from an internal system.
To solve the lab, change the stock check URL to access the admin interface at http://localhost/admin and delete the user carlos. 
![before solve this lab](image/ssrf1.png)
to solve this lab use burpsuite and change the stockApi to stockApi=http://localhost/admin to delete carlos
 stockApi=http://localhost/admin/delete?username=carlos
![proses to solve the lab](image/ssrf2p.png)
The Lab is Solved 
![Solved](image/ssrf1s.png)