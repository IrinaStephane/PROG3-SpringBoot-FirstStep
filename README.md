# <div align="center">⚡ Spring Boot REST Service: Getting Started ⚡</div>
This is a foundational project demonstrating how to build a simple RESTful Web Service using Java and Spring Boot. The application exposes an endpoint that handles HTTP GET requests and responds with a JSON representation of a greeting.

### 🚀 Features
REST API Endpoint: A functional /greeting mapping.

Dynamic Content: Supports query parameters to personalize the output.

Thread-Safe Counter: Uses AtomicLong to track the number of requests.

Clean Architecture: Separation of concerns between the Controller and the Data Model.

### 🛠️ Requirements
Java 17 or higher

Maven 3.5+

IntelliJ IDEA (or any preferred IDE)

### 📦 Project Structure
Plaintext
```
src/main/java/com/example/restservice/
├── RestServiceApplication.java  # Main entry point
├── Greeting.java               # Data model (POJO)
└── GreetingController.java     # REST Controller handling requests
```

### 🚦 Usage & Testing
Once the server is started (usually on http://localhost:8080), you can test the API using your browser or a tool like Postman.

Default Greeting
URL: http://localhost:8080/greeting

Response:

```JSON
{
"id": 1,
"content": "Hello, World!"
}
```
Personalized Greeting
URL: http://localhost:8080/greeting?name=User

Response:

```JSON
{
"id": 2,
"content": "Hello, User!"
}
```