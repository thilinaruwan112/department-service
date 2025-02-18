# Department Service

## Description
The Department Service is part of a Spring Boot application that manages department-related functionality such as adding, updating, deleting, and fetching department details. It is built using Java, Spring Boot, and integrates with a MySQL database.

## Features
- Create a department
- Retrieve department details
- Update department information
- Delete a department

## Technologies Used
- **Spring Boot**: For building the REST API and backend logic.
- **JPA (Java Persistence API)**: For interacting with the MySQL database.
- **H2 Database**: (Or MySQL if preferred) for persistence.
- **Lombok**: For reducing boilerplate code.
- **Maven**: For managing dependencies and building the project.

## Getting Started

### Prerequisites
- Java 17 or later
- Maven
- MySQL (or H2 for in-memory database)

### Setup Instructions

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/department-service.git
   ```

2. Navigate to the project directory:
   ```bash
   cd department-service
   ```

3. Update the `application.properties` or `application.yml` to configure the database connection if using MySQL:
   ```properties
   spring.datasource.url=jdbc:mysql://localhost:3306/your_database_name
   spring.datasource.username=your_username
   spring.datasource.password=your_password
   ```

4. Install dependencies and run the application:
   ```bash
   mvn clean install
   mvn spring-boot:run
   ```

## Endpoints

* **POST** `/departments` - Create a new department
    * Request Body:
      ```json
      {
          "name": "Human Resources",
          "location": "New York"
      }
      ```
* **GET** `/departments/{id}` - Get department details by ID
* **PUT** `/departments/{id}` - Update department details by ID
* **DELETE** `/departments/{id}` - Delete department by ID

## License
This project is licensed under the MIT License - see the LICENSE file for details.
