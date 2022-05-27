# Taxi Service
![image](src/main/resources/taxi.jpg)

# Mission
* Create a taxi service with authentication system

![line](src/main/resources/rainbow.png)
# How to start
* During the first launch you will be redirected to a login page where you have two options: login (if you already registered)
  or register like a new driver
* To use all features you need to create new driver and authenticate
* Driver can add himself to different cars
* The remaining functionality you can find by starting the app

![line](src/main/resources/rainbow.png)
## Implementation details and technologies
Project based on 3-layer architecture:
* Presentation layer (controllers)
* Application layer (services)
* Data access layer (DAO)

![line](src/main/resources/rainbow.png)
## Technologies 
* Apache Tomcat
* MySQL
* Servlet
* JSP
* JDBC
* JSTL
* HTML, CSS

![line](src/main/resources/rainbow.png)
## Setup
* Install IntelliJ IDEA, MySQL and MySQL Workbench
* Configure Apache Tomcat
* Create a schema and all the necessary tables by using the script from `resources/init_db.sql` in MySQL Workbench
* In the `/util/ConnectionUtil.java` class change the "user" and "password" properties to the ones you specified when installing MySQL
```java
    private static final String URL = "YOUR URL";
    private static final String USERNAME = "YOUR USERNAME";
    private static final String PASSWORD = "YOUR PASSWORD";
    private static final String JDBC_DRIVER = "YOUR DRIVER";
```
* In the `src/main/resources/log4j2.xml` at line `File name = "File" fileName = "logs\app.log"` replace `"logs\app.log"` with absolute path to `.log` file
* Configure TomCat Local server `(Add New Configuration -> TomCat -> Local -> Fix -> taxi-service : war exploded -> OK)`
* Start the application

![line](src/main/resources/rainbow.png)
