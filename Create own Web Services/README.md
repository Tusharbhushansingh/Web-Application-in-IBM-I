# Create Web Services in IBM i
Step 1:- Firstly update the Configuration file of Apache Server as shown below.

         ScriptAliasMatch /tushar/([a-z0-9]+)/.* /Qsys.Lib/Tushar.Lib/$1.pgm   
         <Directory /Qsys.Lib/Tushar.Lib>                                      
         order allow,deny                                                    
         allow from all                                                      
         SetEnv QIBM_CGI_LIBRARY_LIST "TUSHAR"                               
         </Directory>            
         
 ![image](https://user-images.githubusercontent.com/42302678/107846042-85e26d00-6e06-11eb-827d-1ff8c68e1f11.png)
 
 Step 2:- Create a new program to connect you IBM i to Web Browser. You can take reference from below link or *Code to Create own Web Services.txt*.
 
 link:- [title](https://github.com/Tusharbhushansingh/Web-Application-in-IBM-I/blob/main/Create%20own%20Web%20Services/Code%20to%20create%20own%20web%20Services.txt)
 
 Step 3:- Compile your program using option 15 and make it module.
 
 Step 4:- Bind your program with QZHBCGI and QC2LE services program by using below command.
 
    CRTPGM PGM(TUSHAR/RPG03) MODULE(TUSHAR/RPG03) BNDSRVPGM((QHTTPSVR/QZHBCGI) (QHTTPSVR/QC2LE)) 
    
 Step 5:- Open Web browser and enter your as400 IP/tushar/RPG03/1 in the URL and your customize web services will appear in XML format as shown below.
 
 ![image](https://user-images.githubusercontent.com/42302678/107846224-14a3b980-6e08-11eb-82fd-7ffa4c19d8f2.png)
 
 
