# 🎥 Cinema-app 
>Application that simulates a cinema service with the shopping cart and orders.
>Supports authentication, registration and CRUD operations with user, order, shopping cart, movie, movie session and cinema hall.

## 📃 Content
- [How to start using](https://github.com/ira0807/cinema-app#-how-to-start-using)
- [Project structure](https://github.com/ira0807/cinema-app#-project-structure)
- [Features](https://github.com/ira0807/cinema-app#-features)
- [Technologies](https://github.com/ira0807/cinema-app#-technologies)

## ⚙ How to start using

1. Fork this repositories
2. Copy link of project
3. Open new project from Version Control and clone it
4. Edit `db.properties` file in `resources` - write your own data:
```bash
   db.driver=YOUR_DRIVER
   db.url=YOUR_URL
   db.user=YOUR_USERNAME
   db.password=YOUR_PASSWORD
```
Example:
```bash
   db.driver=com.mysql.cj.jdbc.Driver
   db.url=jdbc:mysql://localhost:3306/cinema-app?serverTimezone=UTC
   db.user=bob
   db.password=12345
```
5. Install [Tomcat](https://archive.apache.org/dist/tomcat/)
6. Configure Tomcat server in your IDEA
7. Run project

>HINT: for testing of methods you can use [Postman](https://web.postman.co/) and writing parameters in the body

## 🧬 Project structure
>The project has an N-Tier Architecture:

- Controller - accept requests from clients and display information in browser
- Service - contains all the business logic of our application
- DAO - is responsible for communicating with the database

## 🎯 Features
- Log in/out
- Registration/Authentication user
- Distribution of roles and access (Admin/User)
- Admin access:
- - **add** new cinema hall
- - **get** list of cinema halls
- - **add** new movie
- - **get** list of movies
- - **add/update/delete** movie session
- - **get** list of available movie sessions
- - **get** user by his email
- User access:
- - **get** list of cinema halls
- - **get** list of movies
- - **get** list of available movie sessions
- - **get** list of orders
- - **complete** new order
- - **update** movie session in shopping cart
- - **get** shopping cart by user

## 💻 Technologies
- [Java 11](https://www.oracle.com/java/technologies/downloads/)
- [Maven](https://maven.apache.org/download.cgi)
- [MySQL](https://dev.mysql.com/downloads/installer/)
- [Tomcat (9.0.50)](https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.50/bin/)
- JPA/Hibernate
- Spring MVC
- Spring Security
