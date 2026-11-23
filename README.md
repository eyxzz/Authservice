# Authservice

Authentication and authorization service built with **Java 27**, **Spring Boot 4.2.0**, **Spring Security**, **JWT (`java-jwt`)**, **Spring Data JPA**, and **SQL**.

## Project Structure (`me.eyxz.authservice`)

* `config`: security configuration (`SecurityConfig`), JWT filter (`JwtFilter`), and token generation/validation (`TokenService`).
* `controller`: authentication endpoints (`/auth/register`, `/auth/login`) and user retrieval endpoint (`/users`).
* `model`: `User` entity implementing `UserDetails`.
* `repository`: data access layer with `UserRepository` backed by SQL.

## How to Run

1. Configure your SQL datasource and token secret in `src/main/resources/application.properties`.
2. Reload Maven dependencies from `pom.xml`.
3. Run `AuthserviceApplication`.
