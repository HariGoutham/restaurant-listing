# Spring Boot Application Guide (restaurant listing service)

## What You Need

Before starting, make sure you have the following installed:

- **Java JDK 17 or higher** (to run Java programs)
- **Maven 3.6.x or higher** (to build the project)
- **Git** (optional, to download the code)
- **Docker** (optional, to run the app in a container)

## How to Set Up

### 1. Download the Code
```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

### 2. Build the Application:
```bash
mvn clean install
```

### 3. application.properties or application.yml in the src/main/resources folder.

- **spring.datasource.url=jdbc:mysql://localhost:3306/your-database**
- **spring.datasource.username=your-username**
- **spring.datasource.password=your-password**

### 4. Run the Application
```bash
mvn spring-boot:run
```

### 5. Run with Docker:
```bash
docker build -t your-app-name .
docker run -p 8080:8080 your-app-name
```

### 6. Access the App:
http://localhost:8080

### 7. Run Tests
```bash
mvn test
```

### 8. With Docker:
Push the Docker image to a registry (like Docker Hub) and deploy it to your server.

