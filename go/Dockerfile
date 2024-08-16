# Use the official Golang image from the Docker Hub
FROM golang:1.18-alpine

# Set the working directory
WORKDIR /app

# Copy the go.mod and go.sum files
COPY go.* ./

# Download the Go module dependencies
RUN go mod download

# Copy the rest of the application code
COPY . .

# Build the Go application
RUN go build -o /hello-world-go

# Expose the port your app runs on
EXPOSE 3000

# Command to run the application
CMD ["/hello-world-go"]
