# Hello World Spring Boot

A simple "Hello, World!" RESTful web service built using Spring Boot.

## Getting Started

These instructions will help you set up and run the project on your local machine and in a Docker container.

### Prerequisites

You need to have the following installed on your system:

- Java Development Kit (JDK 8 or later)
- Apache Maven
- Docker

### Installation

**Build the Project:**

```bash
mvn clean package
```

### Dockerization

The project includes a `Dockerfile` to build and run the application in a Docker container.

1. **Build the Docker Image:**

Make sure you are in the project directory.

```bash
docker build --no-cache -t hello-world-spring-boot:v1 .
```

2. **Run the Docker Container:**

```bash
docker run -p 3000:3000 hello-world-spring-boot:v1
```

3. **Access the Web Service:**

Open your web browser and navigate to `http://localhost:3000`, and you should see the message "Hello, World!".
