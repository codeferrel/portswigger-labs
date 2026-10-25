Lab: DOM XSS in innerHTML sink using source location.search
![before_solve](image/xssbefore3.png)
to solve this lab we use payload we use payload <img src=1 onerror=alert(1)> and
This DOM XSS vulnerability happens because the innerHTML sink parses your input string as active HTML code, and the <img src=1 onerror=alert(1)> payload bypasses the browser's built-in defenses that block standard <script> tags when using innerHTML. [1] 
![find_xss](image/xss3proses.png)
and finnaly the Lab is solved

![After_solve](image/xss3aftersolve.png)