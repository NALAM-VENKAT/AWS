# Sample Maven Web Application

A minimal JSP web application packaged as a WAR file with Apache Maven. It is intended for the AWS EC2 + Docker + Tomcat deployment assignment.

## Project layout
- `pom.xml`: Maven configuration; packaging is `war`.
- `src/main/webapp/index.jsp`: homepage served by Tomcat.

## Build locally (optional)
Requires JDK 11 and Maven:
```bash
mvn clean package
```

The build creates `target/sample-webapp.war`.

## Deployment plan
Push this project to the GitHub repository named `AWS`, clone it on the EC2 Ubuntu instance, and create a Dockerfile on the instance to build the WAR with Maven and run it in Tomcat.
