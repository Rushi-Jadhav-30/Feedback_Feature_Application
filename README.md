
# Restaurant Feedback API

This project is a Quarkus-based application for managing restaurant feedback. It includes APIs to create, retrieve, update, and delete feedback records stored in a PostgreSQL database. The API documentation is provided using Swagger UI.

## Table of Contents

- [Getting Started](#getting-started)
- [Prerequisites](#prerequisites)
- [Running the Application](#running-the-application)
- [API Documentation](#api-documentation)
- [Generated Code](#generated-code)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)

## Getting Started

Follow these instructions to get a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

- Java 21 or higher
- Maven 3.6.3 or 
- PG Admin for PostgreSQL 
- Docker (for running PostgreSQL)
- Quarkus CLI (optional, but recommended)

### Running the Application

Clone the dev.rushikeshj.repository

- create Demo_Database in postgres
  - create table FeedbackDetails
  
- create docker image of postgres
  -docker run --name postgres -e POSTGRES_USER=quarkus -e POSTGRES_PASSWORD=quarkus -e POSTGRES_DB=feedback -p 5432:5432 -d postgres:latest
  
-Configure the Database:

 -Update your application.properties file with your database configuration:
   -quarkus.datasource.db-kind=postgresql
   -quarkus.datasource.jdbc.url=jdbc:postgresql://localhost:5432/feedback
   -quarkus.datasource.username=quarkus
   -quarkus.datasource.password=quarkus
   -quarkus.hibernate-orm.database.generation=update

Build and run the application:

./mvnw clean compile quarkus:dev(available at http://localhost:8080)

###API Documentation
-Swagger UI is available for interacting with the API. You can access it at:

--http://localhost:8080/swagger-ui
 

   
