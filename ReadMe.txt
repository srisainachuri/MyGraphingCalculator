How To Run the code:
===============
Step 1: Unzip the file 'MyGraphingCalculator.zip' to a test folder , example: 'C:\graphingCalculator'

Step 2: Download glassfish to C:\graphingCalculator\Test

Step 3: Update 
C:\graphingCalculator\Test\glassfish4\glassfish\config\asenv.bat 
and 
C:\graphingCalculator\Test\glassfish4\glassfish\config\asenv.conf 

The following requires  JDK 1.6 or higher and complete path to jdk install folder.

Find and replace the strings 'C:\Program Files\Java\jdk1.8.0_101' with your system jdk install folder (in both files).

Step 4: Start the server
# start the server
C:\graphingCalculator\Test\glassfish4\bin\asadmin.bat start-domain

Step 5: Launch the C:\graphingCalculator\Test\mainWindow.py to run the calculator.