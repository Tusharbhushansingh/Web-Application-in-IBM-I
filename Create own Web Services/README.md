# Create Web Services in IBM i
Step 1:- Firstly update the Configuration file of Apache Server as shown below.

         ScriptAliasMatch /tushar/([a-z0-9]+)/.* /Qsys.Lib/Tushar.Lib/$1.pgm   
         <Directory /Qsys.Lib/Tushar.Lib>                                      
         order allow,deny                                                    
         allow from all                                                      
         SetEnv QIBM_CGI_LIBRARY_LIST "TUSHAR"                               
         </Directory>                                                          
