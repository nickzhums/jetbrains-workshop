# Workshop setup

To complete this workshop you will run Spring PetClinic locally, open it in IntelliJ IDEA, and enable GitHub Copilot.

> [!IMPORTANT]
> This repo contains the PetClinic application under [spring-petclinic/](../../spring-petclinic/). All code changes in this workshop happen in that folder.

## Required resources

- A GitHub account
- Access to GitHub Copilot

## Required local installation

### IDE

- IntelliJ IDEA (Community or Ultimate)
- GitHub Copilot plugin installed and signed in (You can directly download it within JetBrains marketplace)

### Local services

- Git (CLI)
- Java 17+

## Run the application

From the repo root, start PetClinic:

- macOS / Linux:

  ```sh
  cd spring-petclinic
  ./mvnw spring-boot:run
  ```

- Windows (PowerShell):

  ```powershell
  cd spring-petclinic
  .\mvnw.cmd spring-boot:run
  ```

Open the app in your browser: http://localhost:8080

## Open the project in IntelliJ

1. Open IntelliJ IDEA.
2. Select **File → Open…**
3. Choose the folder [spring-petclinic/](../../spring-petclinic/) and open it as a project.
4. If prompted, trust the project and allow the IDE to import Maven/Gradle.

## Verify Copilot is active

1. Open **Copilot Chat** (tool window).
2. Start a new chat.
3. Ask: “Explain what this repository is and how I run it locally.”

> [!TIP]
> If Copilot can’t see the project, confirm you’re signed into GitHub in the Copilot plugin and the project has finished indexing.

## Summary and next steps

You now have PetClinic running and the project open in IntelliJ. Next you’ll add a small endpoint to practice Copilot-assisted coding.

| [← Getting started](./README.md) | [Next: Add a simple endpoint →](./1-add-endpoint.md) |
|:--------------------------------|-----------------------------------------------------:|
