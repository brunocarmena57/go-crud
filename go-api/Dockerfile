FROM golang:latest

# Set the Current Working Directory inside the container
WORKDIR /go/src/app

# Copy everything from the current directory to the PWD(Present Working Directory) inside the container
COPY . .

# EXPOSE port 8080 to allow communication to/from server
EXPOSE 8080

# Build the Go app
RUN go build -o main cmd/main.go

# Command to run the executable
CMD ["./main"]