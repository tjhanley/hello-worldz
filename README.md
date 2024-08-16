You are tasked with setting up a simple “Hello World” web application, containerizing it, and deploying it to a Kubernetes cluster using Minikube. You will then update the application to echo the contents of any incoming request and configure a rollout strategy for deploying the updated version.

1. **Build a “Hello World” Web Application:**

   - Choose any programming language you’re comfortable with.
   - Create a simple web application that returns “Hello, World!” when accessed via HTTP.
   - Or chose one of the starting applications

2. **Containerize the Application:**

   - Write a Dockerfile to containerize your web application.
   - Build the Docker image using Docker and push it to DockerHub (or use Minikube’s Docker daemon if you prefer not to push to DockerHub).

3. **Deploy the Application to Minikube:**

   - Create a Kubernetes Deployment YAML file to deploy the containerized application to Minikube.
   - Expose the deployment via a Kubernetes Service, ensuring it’s accessible from outside the cluster (using NodePort or LoadBalancer).
   - Access the application in your browser or via curl/Postman.
