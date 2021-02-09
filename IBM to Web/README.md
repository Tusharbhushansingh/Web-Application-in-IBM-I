# IBM to Web

Step 1: - Run the below command to check the object of QZHBCGI is present in QHTTPSVR or not.

    wrkobj Qhttpsvr/Qzhbcgi

Step 2: - After getting the QZHBCGI object, Check the service program of QHTTPSVR and see the Procedure which we are going to use to communicate our IBM I to Web browser.

    dspsrvpgm Qhttpsvr/Qzhbcgi

**Below is the highlighted Procedure which we are going to use.**

![image](https://user-images.githubusercontent.com/42302678/107365601-08b3b100-6b03-11eb-8ae7-215a66f970e6.png)
 
Step 3: - Create RPGLE program with above procedure. You can take references from the code shared with name RPG01.

Step 4: - Compile the program with module and bind your program with the service **QHTTPSVR/QZHBCGI**

Step 5:- Finally enter your As400 Ip/lib name/program in the URL and Message will be displayed as shown below.

![image](https://user-images.githubusercontent.com/42302678/107364663-bfaf2d00-6b01-11eb-8551-db5a7f1d16b2.png)
 

