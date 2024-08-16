# Hello World Sinatra

A simple "Hello, World!" RESTful API using Sinatra.

## Getting Started

These instructions will help you set up and run the project on your local machine.

### Installation

1. Clone the repository or download the project files.

2. Navigate to the project directory:

   ```bash
   cd path/to/your/project
   ```

3. Build the service:

   ```bash
    docker build -t sinatra-app .
   ```

4. Running the Application

To start the application, run:

    ```bash
    docker run -p 4567:4567 sinatra-app
    ```

5. **Access the Web Service:**

   Open your web browser and navigate to `http://localhost:4567`, and you should see the message "Hello, World!".
