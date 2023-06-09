# Payroll REST API with Spring Boot

This is a simple Payroll Management RESTful API built with Spring Boot. The project demonstrates the core features of Spring Boot, Spring Data JPA, and Spring HATEOAS. 

## Overview

The project provides a basic payroll management system where employees are managed through a RESTful API. It includes the ability to add, update, retrieve, and delete employee records. 

Please note that the functionality for handling orders is incomplete, as the corresponding Order files were removed due to complexities beyond the scope of this initial project.

The project was built using the IntelliJ IDEA development environment, and there's a noteworthy dependency change from `javax` to `jakarta` in import statements.

## Getting Started

The project can be set up with the following steps:

1. Initialize a new Spring Boot project via [Spring Initializr](https://start.spring.io/). 
2. Add Web, H2, and JPA as dependencies.
3. Pull this repository or copy the source code into your project directory.
4. Run the project through your IDE or via the command line with `mvnw spring-boot:run`.

## Testing

To test the API, you can use curl commands in the terminal, or a REST client such as Postman. 

### Sample Requests:

To add a new employee:

curl -X POST localhost:8080/employees -H 'Content-type:application/json' -d '{"name": "Samwise Gamgee", "role": "gardener"}'

To retrieve a list of all employees:

curl localhost:8080/employees


## Future Development

This project serves as a basic implementation of a RESTful API with Spring Boot. Further enhancements can be made by extending the API's functionality to cover additional aspects of payroll management, such as time tracking, payment processing, and more.

In future revisions, the order handling functionality will be revisited and completed.

## Acknowledgements

This project was developed based on the ["Building REST services with Spring"](https://spring.io/guides/tutorials/rest/) tutorial provided by Spring.io.


