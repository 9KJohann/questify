# Hello World Spring Application

This is a simple Spring Boot application that demonstrates a basic "Hello World" functionality. The application is structured to run in a Docker container using Docker Compose.

## Project Structure

```
hello-world-spring
├── src
│   ├── main
│   │   ├── java
│   │   │   └── com
│   │   │       └── example
│   │   │           └── HelloWorldApplication.java
│   │   └── resources
│   │       └── application.properties
├── Dockerfile
├── docker-compose.yml
├── pom.xml
└── README.md
```

## Prerequisites

- Java 11 or higher
- Maven
- Docker
- Docker Compose

## Building the Application

To build the application, navigate to the project directory and run:

```
mvn clean package
```

This will compile the application and create a JAR file in the `target` directory.

## Running the Application with Docker

To run the application using Docker Compose, execute the following command in the project directory:

```
docker-compose up
```

This command will build the Docker image and start the application in a container.

## Accessing the Application

Once the application is running, you can access it at:

```
http://localhost:8080
```

You should see a "Hello World" message displayed in your browser.

## Stopping the Application

To stop the application, you can use:

```
docker-compose down
```

This will stop and remove the containers created by Docker Compose.

## License

This project is licensed under the MIT License.