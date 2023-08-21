# Spring Boot JWT Authentication example with Spring Security & Spring Data JPA

## Dependency
MySQL:
```xml
<dependency>
  <groupId>com.mysql</groupId>
  <artifactId>mysql-connector-j</artifactId>
  <scope>runtime</scope>
</dependency>
```
## Configure Spring Datasource, JPA, App properties
Open `src/main/resources/application.properties`

- For MySQL
```
spring.datasource.url=jdbc:mysql://localhost:3306/userinformation
spring.datasource.username=root
spring.datasource.password=123456

spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQLDialect
spring.jpa.hibernate.ddl-auto=update

# App Properties
sangeet.app.jwtSecret= ======================Sangeet=Spring===========================
sangeet.app.jwtExpirationMs=86400000
```
## Run Spring Boot application
```
On Eclipse, import the project as Maven project and run as Spring Boot Application. It will run on localhost:8082


