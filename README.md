# GitHub Copilot for JetBrains Workshop (Spring PetClinic)

This repository is a hands-on workshop for learning GitHub Copilot **in IntelliJ IDEA** (Copilot for JetBrains), using the **Spring PetClinic** codebase.

The workshop materials live in [content/1-hour/README.md](content/1-hour/README.md).

## Repo layout

- [spring-petclinic/](spring-petclinic/) — upstream Spring PetClinic source (used as the starting point for all exercises)
- [content/](content/) — workshop instructions and reusable prompts
- [.github/copilot-instructions.md](.github/copilot-instructions.md) — repository-wide Copilot instructions (students will extend this during the workshop)

## Prerequisites

- A GitHub account with access to GitHub Copilot
- IntelliJ IDEA (Community or Ultimate)
- Git
- Java 17+

## Quick start (run the app)

From the repo root:

- macOS / Linux:
	- `cd spring-petclinic && ./mvnw spring-boot:run`
- Windows (PowerShell):
	- `cd spring-petclinic; .\mvnw.cmd spring-boot:run`

Then open http://localhost:8080.

## Start the workshop

Follow [content/1-hour/README.md](content/1-hour/README.md).