# Bank API

This is a RESTful API for managing bank accounts. It provides endpoints for creating, reading, updating, and deleting accounts.

## Features

- Create new bank accounts
- Retrieve account information
- Update account information
- Delete bank accounts

## Requirements

- Java 21
- Spring Boot 3.3.4
- MySQL 8.3.0
- Maven 3.13.0

## Configuration

Ensure that you have set up your MySQL database properly and updated the application.properties (or application.yml) file with the correct database credentials:

```
spring.datasource.url=jdbc:mysql://localhost:YOUR_PORT/YOUR_DATABASE
spring.datasource.username=YOUR_USERNAME
spring.datasource.password=YOUR_PASSWORD
spring.jpa.hibernate.ddl-auto=update
```

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/bank-api.git
   ```
2. Navigate to the project directory:

   ```bash
   cd bank-api
   ```
3. Build the project:

   ```bash
   mvn clean install
   ```
4. Run the application:

   ```bash
   java -jar target/bank-api-0.0.1-SNAPSHOT.jar
   ```

## Endpoints
The API provides the following endpoints for managing bank accounts:
   - Create Account
      - POST /accounts
      - Request body: JSON payload with account details

   - Get Account
     - GET /accounts/{id}
      - Retrieves account information by ID.

   - Update Account
      - PUT /accounts/{id}
      - Updates the account information by ID.

   - Delete Account
      - DELETE /accounts/{id}
      - Deletes an account by ID.
