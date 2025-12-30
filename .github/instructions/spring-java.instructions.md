---
applyTo: "**/*.java"
---

# Java + Spring conventions

- Keep changes consistent with Spring PetClinic patterns.
- Prefer Spring MVC controllers + Thymeleaf views unless a JSON API is explicitly requested.
- Use Spring Data repositories for persistence.
- Use constructor injection.
- Prefer Java records only if the project already uses them in similar contexts.
- Keep endpoints and form inputs validated (Bean Validation annotations) when user input is involved.
