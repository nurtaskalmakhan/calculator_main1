# calculator_main1

# Calculator API - Readme
The Calculator API is a simple RESTful API implemented using the Spring Boot framework. It provides basic mathematical operations such as addition, subtraction, multiplication, and division through HTTP endpoints.

# How to Run
Ensure you have Java and Maven installed on your system.
Clone or download the code repository.
Open a terminal and navigate to the project directory.

Run the following command to build the project:
Copy code
mvn clean install

Run the following command to start the application:
arduino
Copy code
mvn spring-boot:run

# API Endpoints
The API exposes the following endpoints:

# GET /add: Performs addition of two numbers.

# Request Parameters:
a (integer): The first number.
b (integer): The second number.
# Response:
Returns the sum of the two numbers as an integer.
GET /subtract: Performs subtraction of two numbers.

# Request Parameters:
a (integer): The first number.
b (integer): The second number.
Response:
Returns the difference between the two numbers as an integer.
GET /multiply: Performs multiplication of two numbers.

# Request Parameters:
a (integer): The first number.
b (integer): The second number.
Response:
Returns the product of the two numbers as an integer.
GET /divide: Performs division of two numbers.

# Request Parameters:
a (double): The dividend.
b (double): The divisor.
Response:
If the divisor is not zero, returns the quotient of the division as a double.
If the divisor is zero, throws an IllegalArgumentException with an error message.
# Usage
Start the application using the instructions mentioned in the "How to Run" section.
Send HTTP GET requests to the appropriate endpoints to perform the desired mathematical operations.
Example: GET http://localhost:8080/add?a=5&b=3 will return 8.
Example: GET http://localhost:8080/divide?a=10&b=2 will return 5.0.
# Dependencies
The project uses the Spring Boot framework, which handles the application configuration, request routing, and REST API functionality.
