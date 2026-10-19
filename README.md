# Glory Textile – Inventory Management System

## 📌 Project Overview

**Glory Textile** is an Inventory Management System developed to simplify and streamline inventory-related operations in the textile industry. The application manages materials, vendors, and inventory information through a microservices-based architecture.

The project uses Spring Boot for backend development, React for the frontend, and MySQL for database management. It also incorporates CI/CD practices, Docker containerization, and code quality analysis to improve the development and deployment process.

## 🎯 Objectives

- Digitize and simplify inventory management operations.
- Maintain and manage material and vendor information.
- Enable communication between independent microservices.
- Provide a user-friendly interface for inventory-related activities.
- Improve software quality through automated testing and code analysis.
- Streamline application builds and deployment using DevOps tools.

## ✨ Key Features

- **Inventory Management:** Manage inventory-related information.
- **Material Management:** Maintain material records and related details.
- **Vendor Management:** Organize and manage vendor information.
- **REST API Integration:** Enable communication between the frontend and backend services.
- **Microservices Architecture:** Separate application responsibilities into independent services.
- **Database Integration:** Persist application data using MySQL.
- **CI/CD Pipeline:** Automate build and integration activities.
- **Docker Support:** Build container images for application deployment.
- **Code Quality Analysis:** Use SonarQube to analyze code quality and JaCoCo to measure test coverage.

## 🛠️ Technology Stack

| Category | Technologies |
|---|---|
| Frontend | React.js, JavaScript, HTML, CSS |
| Backend | Java, Spring Boot |
| Architecture | Microservices |
| API Communication | REST APIs, RestTemplate |
| Database | MySQL |
| Build Tool | Maven |
| Containerization | Docker |
| CI/CD | Jenkins |
| Code Quality | SonarQube |
| Code Coverage | JaCoCo |
| Version Control | Git, GitHub |

## 🏗️ System Architecture

The application follows a microservices architecture in which different backend services handle specific responsibilities.

- **Frontend:** Provides the user interface and sends HTTP requests to the backend.
- **Inventory Management Service:** Handles inventory-related business operations and coordinates with the required services.
- **Material Service:** Manages material-related data and operations.
- **Vendor Service:** Manages vendor-related data and operations.
- **Database:** Stores application data in MySQL.
- **CI/CD Pipeline:** Supports automated building, testing, code analysis, and Docker image creation.

## 🔄 Application Workflow

1. The user interacts with the React frontend.
2. The frontend sends HTTP requests to the appropriate backend REST API.
3. The Spring Boot controller receives and processes the incoming request.
4. The service layer executes the business logic.
5. The repository layer communicates with the database.
6. The application retrieves or updates the required information.
7. The backend returns an HTTP response to the frontend.
8. The frontend displays the result to the user.

When data from another microservice is required, the relevant service communicates with that microservice through REST APIs.

## ⚙️ Prerequisites

Install the following software before running the project:

- Java Development Kit (JDK)
- Node.js and npm
- MySQL Server
- Maven
- Git
- Docker (for containerization)
- Jenkins and SonarQube (for CI/CD and code quality analysis)

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone <YOUR_GITHUB_REPOSITORY_URL>
cd <YOUR_PROJECT_FOLDER>
```

Replace the placeholders with your actual repository URL and project directory.

### 2. Configure the Database

Create a MySQL database and configure the database connection in the relevant Spring Boot service's `application.properties` file.

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/materialdb
spring.datasource.username=YOUR_USERNAME
spring.datasource.password=YOUR_PASSWORD

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
```

Update the database name and credentials according to each service's configuration.

### 3. Run the Backend Services

Open each Spring Boot microservice separately in your IDE.

Run the main application class or use Maven:

```bash
mvn clean install
mvn spring-boot:run
```

Repeat these steps for the Inventory Management, Material, and Vendor services. Configure the required ports and service URLs before starting the application.

### 4. Run the Frontend

Navigate to the frontend directory:

```bash
cd frontend
npm install
npm start
```

Use the command supported by your frontend project's configuration. For Vite-based projects, the command may be `npm run dev`.

### 5. Access the Application

Open the local URL displayed by the frontend development server. Ensure the backend services and MySQL database are running.

## 🔧 DevOps and CI/CD

The project incorporates DevOps practices to improve build automation, testing, and application quality.

- **Maven:** Manages dependencies and builds the Spring Boot applications.
- **Jenkins:** Supports automated CI/CD pipeline execution.
- **Docker:** Creates container images for application packaging.
- **SonarQube:** Analyzes source code for maintainability and potential quality issues.
- **JaCoCo:** Generates code coverage reports to evaluate test coverage.

## 🧪 Testing and Quality Assurance

The project uses code quality and coverage tools as part of its development workflow.

- Run automated tests using the project's configured testing framework.
- Generate coverage reports using JaCoCo.
- Analyze source code with SonarQube.
- Review build and quality-gate results to identify areas for improvement.

## 🔮 Future Enhancements

- Add role-based authentication and authorization.
- Introduce inventory alerts for low-stock materials.
- Generate inventory and vendor reports.
- Implement advanced search and filtering.
- Integrate cloud deployment and monitoring.
- Expand automated testing and improve code coverage.

## 👨‍💻 Project Type

**Capstone Project – Glory Textile Inventory Management System**

Developed as a practical application of full-stack development, Spring Boot microservices, database integration, and DevOps practices.

## 📄 License

This project is intended for educational and demonstration purposes. Add an appropriate open-source license if you plan to distribute the source code publicly.
