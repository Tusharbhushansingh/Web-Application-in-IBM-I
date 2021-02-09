# Web-Application-in-IBM-I
Step 1: - Check the Http Server is installed or not in your system by running below command.
                WRKACTJOB SBS(QHTTPSVR)
 
Step 2: - If not Http Server is not installed then run below command.
STRTCPSVR *HTTP HTTPSVR(*ADMIN)

Step 3: -Start the Apache server by running below command.
STRTCPSVR SERVER(*HTTP) HTTPSVR(APACHEDFT)

Step 4: - Go to Brower and enter your as400 IP/index.html in the URL.
 
Step 5: - To create your own Web page, Open directory /www/apachedft/conf and your directory by using Alias as shown below.
Alias /mydocs/ /Home/Tushar/
<Directory /Home/Tushar>                           
  order allow,deny                                                     
  allow from all                                                       
</Directory>    
 
Step 6: - Restart the Apache Server by below command.
STRTCPSVR SERVER(*HTTP) RESTART(*HTTP) HTTPSVR(APACHEDFT)

Step 7: - Create new Directory in Home by using below command.
CRTDIR DIR('Home/Tushar')

Step 8: - Add the Html code in your Directory. Ex- Home/Tushar/Welcome.html.
 
Step 9: - Go to Browser and enter your as400 IP/mydocs/welcome.html in the URL and your customize web page will appear.      


