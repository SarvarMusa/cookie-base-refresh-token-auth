# Spring Boot Cookie-Based JWT Refresh Token Authentication

[![CI](https://github.com/SarvarMusa/cookie-base-refresh-token-auth/actions/workflows/ci.yml/badge.svg)](https://github.com/SarvarMusa/cookie-base-refresh-token-auth/actions/workflows/ci.yml)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

A robust Spring Boot backend demonstrating secure cookie-based JWT authentication with refresh tokens. This architecture prevents common vulnerabilities such as XSS and CSRF by storing the JWT in an `HttpOnly` cookie rather than local storage.

## 🚀 Tech Stack

- **Framework:** Spring Boot 3
- **Language:** Java 17
- **Security:** Spring Security & JJWT
- **Database:** MySQL & Spring Data JPA
- **Build Tool:** Maven

## 🔒 Security Features

- **HttpOnly Cookies:** JWT tokens are stored in HttpOnly cookies to protect against Cross-Site Scripting (XSS) attacks.
- **Refresh Tokens:** Short-lived access tokens with secure refresh token rotation.
- **Stateless Authentication:** Fully stateless REST API using JWT.
- **Environment Driven:** Configuration driven by environment variables for enhanced security.

## 🛠️ Getting Started

### Prerequisites

- Java 17
- Maven 3.6+
- MySQL 8

### Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/SarvarMusa/cookie-base-refresh-token-auth.git
   cd cookie-base-refresh-token-auth
   ```

2. **Configure Database & Secrets:**
   Set the following environment variables (or update `application.properties`):
   - `DB_PASSWORD` (Your MySQL Password)
   - `JWT_SECRET` (A strong, randomly generated hex string for JWT signing)

3. **Run the application:**
   ```bash
   ./mvnw spring-boot:run
   ```

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
