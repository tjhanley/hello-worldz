# Hello World FastAPI

A simple "Hello, World!" RESTful API using FastAPI.

### Installation

1. Clone the repository or download the project files.

2. Navigate to the project directory:

```bash
cd path/to/your/project
```

3. Build the service:

```bash
docker build --no-cache -t fastapi-poetry-app:v1 .
```

4. Running the Application

To start the application, run:

```bash
docker run -d -p 3000:3000 fastapi-poetry-app:v1
```

5. **Access the Web Service:**

Open your web browser and navigate to `http://localhost:3000`, and you should see the message "Hello, World!".
