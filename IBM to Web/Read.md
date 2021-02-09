#IBM I to Web Browser

Step 1: - Run the below command to check the object of QZHBCGI is present in QHTTPSVR or not.

                       wrkobj Qhttpsvr/Qzhbcgi

Step 2: - After getting the QZHBCGI object, Check the service program of QHTTPSVR and see the Procedure which we are going to use to communicate our IBM I to Web browser.
dspsrvpgm Qhttpsvr/Qzhbcgi
Below is the highlighted Procedure which we are going to use.
 
Step 3: - Create RPGLE program with above procedure. You can take references from the code shared with name RPG01.
Step 4: - Compile the program with module and bind your program with the service of QHTTPSVR/QZHBCGI
Step 5:- Finally enter your As400 Ip/lib name/program in the URL and Message will be displayed as shown below.
 
