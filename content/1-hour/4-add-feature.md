# Add a pet adoption feature (Agent Mode)

## Scenario

PetClinic handles veterinary visits, but the clinic also wants to help the community with **pet adoption postings**.

You will add a new “Adoptions” feature that supports:

- **People posting a pet for adoption** (create and manage a listing)
- **People who want to adopt** (browse listings and submit an application)

This is a multi-file feature: domain model, persistence, web pages, and (ideally) tests.

## Use Agent Mode

In this part, use **Copilot Agent Mode** (if your Copilot for JetBrains UI exposes it).

- If you see a mode selector like **Ask / Edit / Agent**: choose **Agent**.
- If your JetBrains Copilot client does not have Agent Mode yet, use the same prompt but work iteratively:
  - have Copilot propose a plan
  - apply changes in smaller chunks
  - run tests between chunks

> [!IMPORTANT]
> Even in Agent Mode, you are responsible for reviewing the diffs and validating the app.

## Acceptance criteria (keep it minimal)

### UI navigation

- Add a new top-level navigation item: **Adoptions**
- The feature should use server-rendered pages (Thymeleaf), consistent with PetClinic.

### Adoption listings (posting a pet)

- A page to list adoption listings
- A page to create a listing with fields:
  - pet name (required)
  - pet type (required; reuse PetClinic pet types if feasible)
  - description (required)
  - location/city (required)
  - contact email (required)
  - status: AVAILABLE / ADOPTED (default AVAILABLE)

### Adoption applications (want to adopt)

- From a listing details page, a user can submit an application with fields:
  - applicant name (required)
  - email (required)
  - phone (optional)
  - message (required)
- After submitting, redirect back to the listing with a success message.

### Data / persistence

- Persist the new entities using Spring Data JPA
- Use the default H2 database profile for local development

### Tests (recommended)

- Add at least one controller test or repository test for the new feature.

## Runbook

- Start the app:
  - Windows PowerShell: `cd spring-petclinic; .\mvnw.cmd spring-boot:run`
  - macOS/Linux: `cd spring-petclinic && ./mvnw spring-boot:run`
- Run tests:
  - `cd spring-petclinic && ./mvnw test`

## Agent prompt

Open the prompt file and use it as your Agent Mode request:

- [../prompts/agent-add-adoptions.md](../prompts/agent-add-adoptions.md)

> [!TIP]
> Don’t treat the prompt as magic. Read it, edit it, and add constraints based on what you want.

## Summary and next steps

You’ve used Agent Mode (or an agent-like workflow) to add a real multi-file feature. Next is a bonus exercise combining Agent Mode with tighter custom instructions.

| [← Copilot instructions](./3-copilot-instructions.md) | [Next: Bonus (Agent Mode + instructions) →](./5-bonus.md) |
|:-----------------------------------------------------|----------------------------------------------------------:|
