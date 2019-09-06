How To Run:
===============
Step 1: Unzip the file 'MyGraphingCalculator.zip' to a test folder , example: 'C:\graphingCalculator'

Step 2: Download and install glassfish 4.x to C:\graphingCalculator\Test
https://download.oracle.com/glassfish/4.0/release/glassfish-4.0-windows.exe

Step 3: Update 
C:\graphingCalculator\Test\glassfish4\glassfish\config\asenv.bat 
and 
C:\graphingCalculator\Test\glassfish4\glassfish\config\asenv.conf 

The following requires  JDK 1.6 or higher and complete path to jdk install folder.

Find and replace the strings 'C:\Program Files\Java\jdk1.8.0_101' with your system jdk install folder (in both files).

Step 4: Start the server
# start the server
C:\graphingCalculator\Test\glassfish4\bin\asadmin.bat start-domain

Step 5: Deploy the war file MyGraphingCalculator.war to glassfish instance (see doc for sample/details :https://docs.oracle.com/cd/E19798-01/821-1757/ghgjj/index.html)
Below sample run, correct the path of glassfish install bin folder and MyGraphingCalculator.war location
C:\graphingCalculator\Test\glassfish4\bin\asadmin.bat deploy C:\graphingCalculator\MyGraphingCalculator\dist\MyGraphingCalculator.war

Step 6: Test the deployment by accessing the restful webservice end point in web browser. See sample url below
http://localhost:8080/graphingCalculator/webresources/math?mathExpresion=x^2&variable=x&domain=1,10&intergralLimits=1,1

Step 7: Launch the C:\graphingCalculator\Test\mainWindow.py to run the calculator.