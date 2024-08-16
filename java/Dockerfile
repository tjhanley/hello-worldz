# Use the official OpenJDK as a parent image
FROM openjdk:8-jdk-alpine

# Set the working directory
WORKDIR /app

# Copy the Maven Wrapper and project files to the container
COPY .mvn/ .mvn
COPY mvnw pom.xml ./

# Download dependencies
RUN ./mvnw dependency:resolve

# Copy the rest of the project files
COPY src ./src

# Build the application
RUN ./mvnw package

# Expose port 3000
EXPOSE 3000

# Run the application
CMD ["java", "-jar", "target/hello-world-spring-boot-1.0-SNAPSHOT.jar", "--server.port=3000"]
