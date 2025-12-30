# Copilot instructions (repo-wide + custom)

## Scenario

As you move from small changes to multi-file features, Copilot works best when it understands your project’s conventions: testing style, architecture boundaries, and where code should go.

In this exercise you will:

- add a repo-wide Copilot instructions file
- add a more specialized instructions file for Java/Spring
- practice “basic file addition” via Copilot

## What are Copilot instructions?

Copilot instructions live in `.github/copilot-instructions.md`. They provide **project-wide** context and conventions that should apply for all developers.

> [!IMPORTANT]
> Keep instructions concise. Very large instruction files can drown out relevant code context.

## Step 1: Create/update the repo-wide instructions

Open `.github/copilot-instructions.md` and review the defaults.

Then, in Copilot Chat, ask it to improve the file for this repo. Example prompt:

```
Update .github/copilot-instructions.md for this repo.
Include: Java 17+, Spring Boot MVC + Thymeleaf, Spring Data JPA.
Prefer Maven wrapper commands, add testing expectations (JUnit), and keep it concise.
```

Review the changes and keep what matches your team’s style.

## Step 2: Add specialized instructions (custom)

This repo also includes specialized instructions under `.github/instructions/`.

These are intended to be more specific than the repo-wide file. Depending on your Copilot client, they can be applied by pattern or added to chat context.

- `.github/instructions/spring-java.instructions.md`
- `.github/instructions/tests-java.instructions.md`
- `.github/instructions/thymeleaf.instructions.md`

Try asking Copilot to implement a tiny helper (as a practice task) while following these rules.

## Step 3: Practice “basic file addition” with Copilot

Ask Copilot to create a new file (don’t write it yourself). Example:

```
Create a new package-info.java for org.springframework.samples.petclinic explaining, in 5-8 lines, the overall package structure. Keep it accurate and minimal.
```

Then review the output and ensure:

- the file is placed correctly
- the doc matches the repo
- it doesn’t invent packages/classes

## Summary and next steps

You’ve improved Copilot’s default context so it can work more reliably across multiple files. Next you’ll build a new adoption feature using **Agent Mode**.

| ← Explore the project | Next: Add adoption feature (Agent Mode) → |
|:----------------------|------------------------------------------:|
