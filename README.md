🔧 HOW TO RUN STUDYSMART PROJECT USING TOMCAT (STEP BY STEP)
✅ STEP 1: INSTALL JAVA (JDK)

First check if Java is already installed:

Open Command Prompt and type:

java -version


If version shows → good, skip this step.
If not:

Download JDK 8 or JDK 11

Install it normally (next, next, finish)

Restart PC (yes, really)

Check again:

java -version

✅ STEP 2: DOWNLOAD & INSTALL TOMCAT

Download Apache Tomcat 9 (important, not 10):
https://tomcat.apache.org/download-90.cgi

Download Windows zip (not installer)

Extract it somewhere simple like:

C:\Tomcat\


Inside you should see:

C:\Tomcat\bin
C:\Tomcat\webapps
C:\Tomcat\conf

✅ STEP 3: PUT PROJECT IN TOMCAT

This part people mess up.

Take the project zip (StudySmart.zip)

Extract it

You will get a folder like:

StudySmart


COPY this folder into:

C:\Tomcat\webapps\


So final path becomes:

C:\Tomcat\webapps\StudySmart\


Inside that should be:

StudySmart
 ├── index.jsp
 ├── class.jsp
 ├── profile.jsp
 ├── WEB-INF
 ├── css
 ├── js


If WEB-INF is missing, Tomcat won’t treat it as web app.

✅ STEP 4: START TOMCAT SERVER

Go to:

C:\Tomcat\bin\


Double click:

startup.bat


A black window opens and stays open.
That means server is running.

If it closes instantly → Java problem.

✅ STEP 5: OPEN PROJECT IN BROWSER

Open Chrome and go to:

http://localhost:8080/StudySmart/


If it opens → project running 🎉
