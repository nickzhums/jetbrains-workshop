# Prompt: Extend Adoptions with constraints

Context:
- Application code is in `spring-petclinic/`.
- Follow repository instructions and specialized instructions under `.github/instructions/`.

Task:
1) Add a minimal “Mark as adopted” capability:
- On the listing details page, add a small form/button to mark listing status as ADOPTED.
- Use POST-redirect-GET.
- Once adopted, hide the application form and show a message that the listing is no longer available.

2) Add a small test:
- Add either a controller test verifying the transition, or a repository/service test verifying status changes.

Constraints:
- Keep it consistent with PetClinic patterns.
- Do not add new dependencies unless required.
- Keep UI changes minimal and accessible.

Process:
- Propose a short plan.
- Implement incrementally.
- Run `./mvnw test` and fix failures.
