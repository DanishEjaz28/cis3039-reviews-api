# Week 11 – Consolidation and Review

## Overview
Week 11 focused on consolidating the cloud-native system developed throughout the module rather than introducing new technical features. The emphasis was on reviewing the existing implementation, ensuring the system was stable, and confirming that core DevOps practices such as CI/CD, automated testing, and environment separation were correctly applied across the project.

## CI/CD Pipeline Review
The backend service uses GitHub Actions to automate build and deployment tasks. Each commit to the main branch triggers a workflow that installs dependencies, builds the project, and deploys the Azure Function App to the configured environment. This ensures that changes are continuously integrated and reduces the risk of manual deployment errors.

The frontend application also includes a GitHub Actions workflow that builds the single-page application and verifies that it compiles successfully. Having automated pipelines for both backend and frontend services reflects good DevOps practice and provides confidence that the system remains deployable at all times.

## Testing and Quality Assurance
Automated testing was reviewed as part of the consolidation process. Unit tests are used to validate core logic and data handling within the backend service, helping to catch regressions early in the development lifecycle. These tests are executed as part of the CI pipeline, ensuring that only code that passes the test suite is deployed.

This approach aligns with the testing pyramid discussed in the lectures, where unit tests form the foundation for maintaining software quality in a cloud-native environment.

## Environment Separation
The system follows a clear separation between development and test environments. Configuration values such as database connections and service endpoints are managed through environment variables, allowing the same codebase to be deployed safely across multiple environments. This separation reduces risk and supports safer experimentation during development.

## Reflection
Week 11 provided an opportunity to reflect on the overall system design and development process. Reviewing the full pipeline highlighted the importance of automation, repeatability, and testing in modern cloud-native applications. The consolidation work confirmed that the system meets the module requirements and follows best practices introduced throughout the course.
