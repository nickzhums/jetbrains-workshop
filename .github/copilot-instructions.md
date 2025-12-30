# Repository instructions (Copilot)

You are helping on a workshop repository that uses the **Spring PetClinic** sample application.

## Project layout

- The application code lives in your local clone of Spring PetClinic.
- Workshop docs and prompt examples live in this workshop repository under `content/`.

## Tech stack

- Java 17+
- Spring Boot (MVC + Thymeleaf)
- Spring Data JPA
- Default database is H2 (in-memory)

## Coding expectations

- Prefer small, reviewable changes.
- Follow existing patterns in PetClinic (controllers, services, repositories, templates).
- Add or update tests when adding behavior.

## Commands

- Run app (macOS/Linux and Git Bash): `./mvnw spring-boot:run`
- Run app (Windows PowerShell): `.\mvnw.cmd spring-boot:run`
- Run tests: `./mvnw test`
