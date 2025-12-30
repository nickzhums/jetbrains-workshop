# Repository instructions (Copilot)

You are helping on a workshop repository that uses the **Spring PetClinic** sample application.

## Project layout

- The application code lives in `spring-petclinic/`.
- Workshop docs live in `content/`.

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

- Run app (macOS/Linux): `cd spring-petclinic && ./mvnw spring-boot:run`
- Run app (Windows PowerShell): `cd spring-petclinic; .\mvnw.cmd spring-boot:run`
- Run tests: `cd spring-petclinic && ./mvnw test`
