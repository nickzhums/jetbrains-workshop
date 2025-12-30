# Prompt: Add an Adoptions feature (PetClinic)

You are working in a local clone of Spring PetClinic (repository root).

Goal: add a minimal Pet Adoption feature to Spring PetClinic using Spring MVC + Thymeleaf + Spring Data JPA.

Constraints:
- Keep changes small and consistent with PetClinic patterns.
- Prefer server-rendered pages (Thymeleaf).
- Use Java 17+.
- Use constructor injection.
- Add at least one test.

Feature requirements:
1) Navigation
- Add a top-level nav link named "Adoptions".

2) Listings (posting a pet)
- Add pages to:
  - list adoption listings
  - create a new listing
  - view a listing details page
- Listing fields:
  - petName (required)
  - petType (required; reuse existing PetClinic pet types if feasible)
  - description (required)
  - city (required)
  - contactEmail (required)
  - status enum: AVAILABLE / ADOPTED (default AVAILABLE)

3) Applications (want to adopt)
- From the listing details page, allow submitting an adoption application:
  - applicantName (required)
  - applicantEmail (required)
  - applicantPhone (optional)
  - message (required)
- After submit, redirect back to listing details and show a success message.

Data/persistence:
- Use JPA entities and Spring Data repositories.
- Ensure it works with default in-memory H2.

Deliverables:
- New entity classes, repositories, controller(s), Thymeleaf templates.
- Update navigation template.
- Add a focused test (controller or repository) to cover core behavior.

Workflow:
- First, inspect the current PetClinic code to find the right patterns for controllers, templates, and navigation.
- Propose a short plan.
- Implement incrementally.
- Run tests and iterate if anything fails.
