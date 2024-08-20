# Hello World Go

A simple "Hello, World!" RESTful API using Go.

## Getting Started

These instructions will help you set up and run the project on your local machine.

### Prerequisites

- [Go](https://golang.org/) (version 1.20 or later)
- Minikube setup

```bash
brew install minikube

minikube start

kubectl config use-context minikube

eval $(minikube docker-env)
```

### Installation

1. Clone the repository or download the project files.

2. Navigate to the project directory:

```bash
cd path/to/your/project
```

3. Build the `v1` image of the service:

```bash
docker build --no-cache -t hello-world-go:v1 .
```

4. Running the Application

To start the application, run:

```bash
docker run -p 3000:3000 hello-world-go:v1
```

5. **Access the Web Service:**

Open your web browser and navigate to `http://localhost:3000`, and you should see the message "Hello, World!".
