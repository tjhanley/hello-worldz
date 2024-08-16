# Hello World Go

A simple "Hello, World!" RESTful API using Go.

## Getting Started

These instructions will help you set up and run the project on your local machine.

### Prerequisites

- [Go](https://golang.org/) (version 1.20 or later)

### Installation

1. Clone the repository or download the project files.

2. Navigate to the project directory:

   ```bash
   cd path/to/your/project
   ```

3. Build the service:

   ```bash
   docker build -t hello-world-go .
   ```

4. Running the Application

To start the application, run:

    ```bash
    docker run -p 8080:8080 hello-world-go
    ```

5. **Access the Web Service:**

   Open your web browser and navigate to `http://localhost:8080`, and you should see the message "Hello, World!".
