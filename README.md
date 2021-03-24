# DeletingOldApplicationLogFiles
This is a Java based application that focuses on deleting the Application old log files which are crossed more than 6months. Once log files are deleted then program will send the automatic alert to technical team. If no files are deleted then will receive the alert like "No files are deleted".  

You can find the code in attached zip file. 

How to Install the program in your local eclipse?

Import the file to another eclipse by right click import -->select existing project in route directory--> then select archive file and give the path name where the file exists or where its saved while exporting. 

How to use the program ?

Export the code as Runnable jar file from Eclipse.
Right click on the Project.
Click on Export.
Create a folder name lib in the desired path For eg: D:\AMI\SchedularJobs\AMIDeleteOldLogs create jar file to the lib folder in desired server.(have attached the jar file in below folder).
Go to the desired location eg: D:\AMI\SchedularJobs\AMIDeleteOldLogs and create a notepad file type the below code(attached bat file in below folder)
echo off
set JAVA_HOME= "C:\Program Files\Java\jre1.8.0_201"
SET CLASSPATH=%CLASSPATH%;.\lib\deletetest.jar;(here give the jar file path)
rem Hit [SPACE] key to continue OR [Ctrl]+[C] to cancel
rem PAUSE
echo on
%JAVA_HOME%\bin\java -Xmx1g deletes.FileDelete
echo off
Save it as .bat file.


