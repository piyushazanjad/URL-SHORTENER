# URL-SHORTENER

Developed an enterprise Java web application using Spring MVC Framework. Used Spring’s JDBC Template to access data in HSQLDB. 
The project includes a signup page where users can create an account with username and password. After the user is logged in, a private page is displayed where users can submit a Long URL and get back a shortened URL. Also, on the same private page, they can view a list of URLs they have shortened and the number of clicks each shortened URL has received. The application also includes a public front page where users can input a shortened URL and view the original URL without following the link. When we
click on the shortened URL, the clicks are recorded before redirecting to the original URL.


Setup Instructions
1. Download and unzip the project on your local drive.
2. Download and keep the build.xml file in web/WEB-INF/Build/build.xml(create a new Build folder in WEB-INF).
3. In the Build folder,
(For ex: \RunningProject\src\main\webapp\WEB-INF\Build)
Open command prompt and type: ant clean.
4. Run the build.xml file as Ant Build.
5. After building the file go to hsqldb manager named manage, run the hsql commands given in the hsqldb command.txt file in the manager. This file contains two create commands which will create two tables for User and Links.
6. In the command prompt of the project folder type: mvn clean . This command will clear all the class files. After doing check the target file you should not have anything in it.
7. Run the mvn package this will create a war in the target subdirectory of the project.
8. Start the tomcat server by Startup.bat command.
9. Deploy the war file to the tomcat manager or copy the war file in the webapps folder of tomcat.
10. Go to this url => http://localhost:8080/RunningProject/login
