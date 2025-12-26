# DotNetApp - .NET Application

CI/CD automated deployment with GitHub Actions (GitFlow).

## Branches (GitFlow)
- main: Production (validated code deployed to PROD)
- develop: Integration branch (has production-ready code from SIT)
- release/*: Release branches for UAT/PROD deployment
- feature/*: Feature branches for development

GitFlow Process:
1. feature/* branches from develop (local development)
2. PR to develop triggers CI/SIT deployment
3. release/* branch from develop for UAT
4. UAT approval triggers deploy
5. PROD approval deploys release to PROD
6. Successful PROD deployment merges to main

