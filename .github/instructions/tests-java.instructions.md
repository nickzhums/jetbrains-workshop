---
applyTo: "**/*Test.java"
---

# Testing conventions

- Prefer focused tests with clear Arrange/Act/Assert structure.
- For Spring MVC controllers, prefer `@WebMvcTest` when possible.
- For repository/data tests, prefer `@DataJpaTest`.
- Use descriptive test names for behavior (not implementation details).
