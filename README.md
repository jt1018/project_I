# project_I
Senior design project being advised by Professor Yao Hu

Setup instructions below:
Getting started with RRCA
 
Verifying for files existence:
Checking files:
 
●  	Download the “RRCA” folder from google documents provided to you.
 
●  	“RRCA” contains two folders inside “Database” and “RRBGUI”.
 
Please check if these files are included inside your “RRCA” folder.
 
●  	“Database” folder contains two SQL files “PCM20200518.sql” and “RRB20200519.sql”.
 
●  	“RRBGUI” folder contains the folders “images”, “lib”, ”RRCA”, “src”, “utility” and the files “comb.rch”, “comb.wel”, “filename.properties”, “h4Cells.txt”, Isratio.txt”, “myclasses.uml”, “Readme”, “streamcell.txt”.
 
●  	“lib” folder contains the files  “commons-collections-3.2.1.jar”,  “commons-math3-3.0.jar”, “jcommon-1.0.16-junit.jar”,  “jcommon-1.0.16.jar”, “jcommon-xml-1.0.16.jar”, “jipopt-3.3.2.jar”, “jipopt.dll”, “mysql-connector-java-5.1.20-bin.jar”, “mysql-connector-java-8.0.19.jar”.
 
Make sure all the files included in this paper exist in your project folder otherwise your program will  not be able to run.
 
Setting up to run the code:
 
Recommended to create a virtual machine.
Downloading Eclipse IDE:
 
●  	Download “Eclipse IDE”. https://www.eclipse.org/downloads/.
 
●  	Install “Eclipse IDE”
 
●  	After Installed your computer will restart.
 
You now installed Eclipse IDE.
Downloading Java runtime environment:
 
●  	Download the jre 1.8 “Windows x86 Offline” https://www.oracle.com/java/technologies/javase-jre8-downloads.html.
 
●  	Install “Windows x86 Offline”.
 
●  	After Installing, restart your computer.
 
You have now installed your Java runtime environment.
 
Setting your Java runtime environment in Eclipse IDE:
 
●  	Open  “Eclipse IDE”.
 
●  	Click in“Window”, “Preferences”, “Java”, “Installed JREs”.
 
●  	Click add, select Standard VM and look for the path where you installed jre 1.8 “Windows x86 Offline”.
 
●  	Click “Apply”.
 
●  	Click in “Window”, “Preferences”, “Java”, “Installed JREs”, “Execution Environments” and select “JavaSE-1.8”.
 
●  	Click “Apply and close”.
 
You have now set your Java runtime environment.
 
Adding your project to Eclipse IDE:
●  	Open “Eclipse IDE”.
 
●  	Go to “File” , “Open project from file system...”.
 
●  	Click in Directory and look for your “RRBGUI”  folder path.
 
●  	Click open folder and then when the file is loaded click finish.
 
You have now opened your project in Eclipse IDE.
 
Adding Libraries to Eclipse IDE:
●  	Open “Eclipse IDE”.
 
●  	Right click in the name of your project.
 
●  	Click in “Properties”.
 
●  	Click in“Libraries” at the top right side of the window.
  
●  	Then select “add JARs” and import the folder “lib” .
 
●  	After the folder “lib” is imported click okay.
 
You have now added the libraries to your project.
 
Changing date in file:
 
●  	Open the folder “RRBGUI” inside “RRCA” in “File browser”.
 
●  	Open the folder “utility” inside “RRBGUI”.
 
●  	Open the file “inputinfo”.
 
●  	Press “Ctrl+F” and search “2006”.
 
●  	Change “2006” to “1995”.
 
●  	Save and exit.
 
 
Adding User Directory to the project:
 
●  	Open “Eclipse IDE”.
 
●  	Click the folder “RRBGUI/src”, then Click in the folder “repRBI” in “Eclipse IDE”.
 
●  	 Open the next clases.
 
●  	“CalDailyRefET.java” and add your “user directory” in lines 355,356.
 
●  	“DbConnection.java” and add your “user directory” in line 41.
 
●  	“ModFlowInput.java” and add your “user directory” in lines 30, 33, 34, 36, 38, 82. 83, 126, 127, 128, 130, 132, 141,146, 147, 228, 244, 245, 247, 248, 251, 252, 254, 255, 264, 279, 281, 291, 292, 295, 296, 297, 300, 301, 302, 333, 334, 335, 338, 339, 340, 341, 342, 343, 344, 345, 346, 347, 348, 350, 351.
 
●  	“RRBProjectViewer.java” and add your “user directory” in line 282.
 
●  	“SFA_Class.java” and add your “user directory” in lines 450, 459,524.
 
●  	Delete “ReadResultsToDB” we will not use this in our project.
 
●  	Open the folder  “RRBGUI/src”, then Click in the folder “Statistics” 
 
●  	Open the next clases.
 
●  	“CountyAgent.java” and add your “user directory” in lines 125, 128, 129, 153, 156, 157, 166, 169.
 
●  	“CountyAgentCloud.java” and add your “user directory” in lines 50, 53, 61, 83, 85, 88, 90.
 
●  	“CountyAgentDaily.java” and add your “user directory” in lines 130, 133, 134, 136, 165, 168, 169, 171, 184, 186, 698, 702, 705.
 
●  	“FeedbackLoop.java” and add your “user directory” in lines 110, 117, 176, 178, 187, 189.
 
You have now added your user directory into the project.
 Creating MySQL server:
The next steps will depend on which visual database design tool the user uses. 
●  	Create a new MySQL server in your visual database design tool (MySQL Workbench, SQLDBM, PhpMyAdmin, DBeaver, etc).
 
●  	Set the server Host as “localhost”.
 
●  	Set the server Port as “3306”.
 
●  	Set the server username as “root”.
 
●  	Set the server password as “198399”.
 
You have now created a MySQL server.
 
Setting username, password, host and port of the server, will match with the information added into databaseinfo.properties file in the project.  
Adding database to server:
●  	Import the database “RRB20200519.sql” from the folder “Database” stored inside the folder “RRCA”.
 
●  	Import the database “PCM20200518.sql” from the folder “Database” stored inside the folder “RRCA”.
 
You have now added the databases into the server.
Checking connection to database:
●  	Open “Eclipse IDE”.
 
●  	Click in “RRBGUI/src”.
 
●  	Click in “repRBI”.
 
●  	Open “Dbconnection.java” class.
 
●  	Run “Dbconnection.java” class.
 
If there are no errors, you have successfully connected to the database.
You have now checked the connection to the database.
 
Running the code:
Running RRBProjectViewer.java:
 
●  	Open “Eclipse IDE”.
 
●  	Click in “RRBGUI/src”.
 
●  	Click in “repRBI”.
 
●  	Open “RRBProjectViewer.java” class.
 
●  	Run “RRBProjectViewer.java” class.
 
 
You have now run the project.

