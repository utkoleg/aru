# Lorby Authentication Service

## Overview

The Lorby Authentication Service is a Spring Boot application that provides user registration, authentication, and verification functionalities. It uses a RESTful API to handle user authentication and verification requests.

## Requirements

- Java 11 or later
- Maven
- Spring Boot
- Lombok

## Getting Started

To get started with the Lorby Authentication Service, follow these steps:

1. **Clone the repository:**

git clone https://github.com/yourusername/lorby-auth.git

markdown
Copy code

2. **Navigate to the project directory:**

cd lorby-auth

markdown
Copy code

3. **Build the project:**

mvn clean install

markdown
Copy code

4. **Run the application:**

mvn spring-boot:run

bash
Copy code

The application will start running on `http://localhost:8080`.

## API Endpoints

The following API endpoints are available:

- **POST /api/v1/auth/register**: Register a new user.
- Request body: `{"username": "your_username", "password": "your_password", "email": "your_email"}`
- **POST /api/v1/auth/authenticate**: Authenticate a user.
- Request body: `{"username": "your_username", "password": "your_password"}`
- **GET /api/v1/auth/verify**: Verify a user's email.
- Request parameter: `?token=your_verification_token`


