# Online Notes Sharing Platform

**Online Notes Sharing Platform** is a simple web application that allows users to create an account and share their notes in text format. Other users can view these notes, making it a convenient tool for knowledge sharing.

## Features

- **User Registration & Login**: Users can create an account to post notes.
- **Post & Share Notes**: Users can add and share text-based notes.
- **View Notes**: Anyone can view the shared notes.
- **Lightweight & Fast**: Built with minimal dependencies for efficiency.

## Tech Stack

- **Backend**: Spring Boot  
- **Frontend**: Thymeleaf  
- **Database**: H2 Database  
- **Build Tool**: Maven  
- **IDE Used**: Eclipse  

## Prerequisites

Ensure you have the following installed before running the project:

- **Java 17** (or a compatible version with Spring Boot)
- **Maven** ([Download Maven](https://maven.apache.org/download.cgi))
- **Eclipse IDE** (or any preferred IDE)

## Setup & Installation

### 1. Clone the Repository

```sh
git clone https://github.com/yourusername/online-notes-platform.git
cd online-notes-platform
```

### 2. Import the Project into Eclipse

1. Open Eclipse.
2. Click on **File > Import**.
3. Select **Existing Maven Projects**.
4. Browse to the project folder and click **Finish**.

### 3. Build the Project Using Maven

```sh
mvn clean install
```

### 4. Running the Application

#### 4.1 Via Maven

```sh
mvn spring-boot:run
```

#### 4.2 Via Eclipse

1. Open the project in Eclipse.
2. Navigate to `OnlineNotesApplication.java` (or the main class with `@SpringBootApplication`).
3. Right-click on the file and select **Run As > Spring Boot App**.

### 5. Accessing the Application

Once the application is running, open your browser and go to:

```
http://localhost:8080
```

### 6. Database Details (H2 Console)

Spring Boot uses an in-memory H2 database. You can access the H2 console for debugging:

1. Open your browser and visit:
   ```
   http://localhost:8080/h2-console
   ```
2. Use the following credentials (if default):
   - **JDBC URL**: `jdbc:h2:mem:testdb`
   - **Username**: `sa`
   - **Password**: *(leave blank or use the configured password in `application.properties`)*

### 7. Configuration (`application.properties`)

Modify `src/main/resources/application.properties` as needed. Example:

```properties
spring.datasource.url=jdbc:h2:mem:testdb
spring.datasource.driverClassName=org.h2.Driver
spring.datasource.username=sa
spring.datasource.password=
spring.h2.console.enabled=true
spring.jpa.database-platform=org.hibernate.dialect.H2Dialect
```

### 8. ORM

This project uses **Spring Data JPA** as the ORM (Object Relational Mapping) framework to manage database interactions efficiently.

## Contributors

- [Sadhanand S S](https://github.com/Sadhanand-SS)

## Feedback

Contributions and suggestions are welcome! Feel free to open an issue or submit a pull request.

