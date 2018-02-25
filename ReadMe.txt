	How To Run:
===============
Step 1: Unzip the file 'standalone.zip' to a test folder , example: 'C:\test'
Step 2: Update the asenv.bat and asenv.conf with 

# The following requires  JDK 1.6 or higher and complete path to jdk install folder
# replace 'C:\Program Files\Java\jdk1.8.0_101' shown below with your system jdk install folder

# add the following to ..\glassfish\config\asenv.bat 
AS_JAVA=C:\Program Files\Java\jdk1.8.0_101
# add the following to ..\glassfish\config\asenv.conf
set AS_JAVA=C:\Program Files\Java\jdk1.8.0_101

Step 3: Start the server
# start the server
C:\test\glassfish4\bin\asadmin.bat start-domain

Step 4: Launch the python script '<replace with the python script name> ' to run the calculator.
