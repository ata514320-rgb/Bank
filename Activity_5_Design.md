```markdown
# Activity 5: Conceptual CI/CD Pipeline Design
‌
## 1. Pipeline Stages
Our pipeline follows these steps:
- Step 1: Build (Creating Docker Image)
- Step 2: Test (Running automated unit tests)
- Step 3: Deploy (Pushing to production)
‌
## 2. Error Handling Scenario
Scenario: What happens if a test fails?
- Action: The pipeline will immediately STOP.
- Error Message: `[ERROR] Unit Test Failed in Module X`.
- Recovery Algorithm:
Developer receives error report.
Developer fixes the code locally.
Developer pushes the new code to trigger a new pipeline.
‌
## 3. Relation between Pipeline and Docker
Docker is used in the Build Stage to ensure that the testing environment is exactly the same as the production environment, preventing "it works on my machine" issues.
```
