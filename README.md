#SpringMVC-REST#

##RESTful web service using Spring 3.1##

This project shows how to build a RESTful web service using Spring 3.1 MVC. It will also demonste the CRUD operation with one of the model object..

###tools and technologies###

* Spring 3.1.0.RELEASE
* jackson-mapper-asl 1.9.9
* jaxb-api 2.2.7
* JDK 1.7
* Tomcat 7.0
* Maven
* Eclipse 

###Project Details###

* Service/Controller
* Model Class
* Spring MVC Context Configuration
* Spring Integration With Web Container
* Application Deployment
* Testing
* Source Code

Complete Tutorial [Web Service with Spring 3.1] (http://www.techiekernel.com/2012/12/restful-web-service-with-spring-31.html)


##AO
Dobra apliakcja do requestów rest: POSTMAN, instalowana przez chromewebapps

GET:
http://localhost:8080/SpringMVC-REST/foobar
[
  {
    "id": 0,
    "name": "ql0",
    "moja_pensja": null
  },
  {
    "id": 1,
    "name": "ql1",
    "moja_pensja": null
  },
  {
    "id": 2,
    "name": "ql2",
    "moja_pensja": null
  },
  {
    "id": 3,
    "name": "ql3",
    "moja_pensja": null
  },
  {
    "id": 4,
    "name": "ql4",
    "moja_pensja": null
  }
]

GET:
http://localhost:8080/SpringMVC-REST/foobar/4
<?xml version="1.0" encoding="UTF-8" standalone="yes"?>
<fooBar>
    <id>4</id>
    <name>ql4</name>
</fooBar>


PUT:
http://localhost:8080/SpringMVC-REST/foobar/3
Headres: Content-Type=application/json
Body:
  {
    "id": 3,
    "name": "ql3",
    "moja_pensja": "100k!"
  }
Response:
  {
    "id": 3,
    "name": "ql3",
    "moja_pensja": "100k!"
  }
  
POST:
http://localhost:8080/SpringMVC-REST/foobar
Headres: Content-Type=application/json
Body:
  {
    "id": 14,
    "name": "q3 rulezzzzzzzzzzzzzzzzzzzzzzz"
  }
Response: true

 DELETE:
 http://localhost:8080/SpringMVC-REST/foobar/3
Response: true  


