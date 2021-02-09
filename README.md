# Web-Application-in-IBM-I
Step 1: - Check the Http Server is installed or not in your system by running below command.

                WRKACTJOB SBS(QHTTPSVR)
                
![image](https://user-images.githubusercontent.com/42302678/107362831-49a9c680-6aff-11eb-94fd-352e13a580bf.png)
 
Step 2: - After running the above command you can see your Http Server subsystem if installed as shown below. 

![image](https://user-images.githubusercontent.com/42302678/107362876-5af2d300-6aff-11eb-816e-be6f7071d7b5.png)
 
Step 3: - If Http Server is not installed then run below command.

               STRTCPSVR *HTTP HTTPSVR(*ADMIN)
               
Step 4: -Start the Apache server by running below command.

               STRTCPSVR SERVER(*HTTP) HTTPSVR(APACHEDFT)
               
Step 5: - Go to Brower and enter your as400 IP/index.html in the URL and below page will appear.

![image](https://user-images.githubusercontent.com/42302678/107362985-82e23680-6aff-11eb-8c49-10dc38f0bde4.png) [image](https://www.google.com)
 
Step 6: - To create your own Web page, Open directory /www/apachedft/conf and add the path of your file in the conf file by using Alias as shown below.

![image](https://user-images.githubusercontent.com/42302678/107363017-91c8e900-6aff-11eb-83b3-3e6fce429a96.png)
 
Step 7: - Restart the Apache Server by below command.

               STRTCPSVR SERVER(*HTTP) RESTART(*HTTP) HTTPSVR(APACHEDFT)

Step 8: - Create new Directory in Home by using below command.

               CRTDIR DIR('Home/Tushar')
               
Step 9: - Add the Html code in your Directory. Ex- Home/Tushar/Welcome.html.

![image](https://user-images.githubusercontent.com/42302678/107363085-aa390380-6aff-11eb-8230-df19d68c6f14.png)
 
Step 10: - Go to Browser and enter your as400 IP/mydocs/welcome.html in the URL and your customize web page will appear as shown below.

![image](https://user-images.githubusercontent.com/42302678/107363118-b91fb600-6aff-11eb-918d-8c0f0d35bf8e.png)
 




