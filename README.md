## #  QuizApp_With_JSP-Servlets
Quiz web application built with JSP, Servlets, and JDBC, with admin and end-user modules integrated

######  Tools required: JSP, Servlet, JDBC, Eclipse IDE, MySQL, and Tomcat 9.

Steps to take in order for the application to work properly:

##### Step 1: Configure the database:
-  Access the MySQL server from the terminal with the command: sudo mysql;

- Then, create a database named quiz with command: create database quiz;
- If the VM has root permissions, create a new user and grant the permissions using the following commands:

```sql
CREATE USER ‘jawadpasha’@‘localhost’ IDENTIFIED BY ‘Jawad@123’;
GRANT ALL PRIVILEGES ON quiz. * TO ‘jawadpasha’@‘localhost’;
```

- Go to the** /db** directory and type **mysql -p quiz quiz.sql** to import the tables and records from the **.sql** file.

##### Step 2: Set up the project with Tomcat and jar files:

- After importing the project into the Eclipse IDE or any other IDE, add a Tomcat server, and the apache-tomcat-9.0.70 version is required for this project. The zip file is available in the **/src/main/webapp/WEB-INF/** directory. Add the library and even include the external jar files from the **/src/main/webapp/WEB-INF/lib/ **directory.

- Update the **DatabaseConnection.java** class in the** src/main/java/** package with the newly created user credentials or your VM MySQL credentials.

##### Step 3: Execute the project:

- Run the project on the server, and the application will be hosted at the following URL: **http://localhost:8080/quiz-app/**

- To access admin dashboard change the URL to: **http://localhost:8080/quiz-app/admin **

- The admin login credentails are:

 ** Email:** admin@gmail.com
  **Password: **12345678

- An excel file containing questions and answers is required to launch the quiz, which can then be completed by end users.
