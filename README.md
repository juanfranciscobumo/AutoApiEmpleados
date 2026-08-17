# Employee API Quality

API test suite built with Java, Serenity BDD, Screenplay, Cucumber and Gradle. It is intended to exercise the Employee API project in the same portfolio.

## What it demonstrates

- API-level BDD scenarios and response assertions
- Screenplay tasks and domain models
- JUnit Platform execution and Serenity reports
- Repeatable CI execution through GitHub Actions

## Run locally

Requirements: JDK 17+ and network access to the configured API environment.

```powershell
.\gradlew.bat clean test aggregate
```

The generated Serenity report is available under `target/site/serenity`.

## Configuration and security

Keep endpoints, credentials, API keys, and personal data outside source control. Store them as CI secrets or environment variables; do not commit `.env`, `.pem`, `.key`, or credential files.
