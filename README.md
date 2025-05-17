# Retail_Online_Banking

## Overview
Alexa Bank is a comprehensive banking application that provides various banking services including account management, ATM card services, loan processing, and customer management. This application is built using Spring Boot and follows a layered architecture.

## Project Structure

```
bank-apps/
├── .mvn/                          # Maven wrapper files
├── src/
│   ├── main/
│   │   ├── java/com/alexa/bank/apps/
│   │   │   ├── controller/        # All controller classes
│   │   │   ├── dto/               # Data Transfer Objects
│   │   │   ├── entity/            # Entity classes
│   │   │   ├── exception/         # Custom exceptions
│   │   │   ├── repo/              # Repository interfaces
│   │   │   └── service/           # Service interfaces and implementations
│   │   └── resources/
│   │       └── application.properties # Configuration file
│   └── test/                      # Test classes
├── .gitignore                     # Git ignore rules
├── LICENSE                        # License file
├── mvnw                           # Maven wrapper script (Unix)
├── mvnw.cmd                       # Maven wrapper script (Windows)
└── pom.xml                        # Maven configuration
```

## Features

### Core Modules
1. **Account Management**
   - Account creation and details management
   - Account balance tracking
   - Random account number generation

2. **Customer Management**
   - Customer registration and profile management
   - Document handling

3. **ATM Services**
   - ATM card management
   - Card details maintenance

4. **Loan Services**
   - Loan application processing
   - Loan details management

5. **Admin Functions**
   - Administrative operations
   - User role management

6. **Authentication**
   - Login functionality
   - Security controls

## Technologies Used

- **Backend**: Spring Boot, Spring Data JPA
- **Database**: (Configured in application.properties)
- **Build Tool**: Maven
- **Java Version**: 8+

## Getting Started

### Prerequisites
- Java JDK 8 or later
- Maven 3.6.0 or later
- Database (MySQL/PostgreSQL/Oracle - as configured in application.properties)

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/amitsahu629/Retail_Online_Banking.git
   ```

2. Navigate to the project directory:
   ```bash
   cd bank-apps
   ```

3. Configure your database settings in `src/main/resources/application.properties`

4. Build the project:
   ```bash
   ./mvnw clean install
   ```

5. Run the application:
   ```bash
   ./mvnw spring-boot:run
   ```

## API Documentation
The application provides REST APIs for all banking operations. API documentation can be accessed after running the application at:
```
http://localhost:8080/swagger-ui.html
```

## Configuration
Edit `src/main/resources/application.properties` to configure:
- Database connection
- Server port
- Application-specific settings

## Testing
To run tests:
```bash
./mvnw test
```

## Contributing
Contributions are welcome. Please fork the repository and create a pull request with your changes.

## License
This project is licensed under the terms of the [LICENSE](LICENSE) file.
