# ⚙️ CI/CD Pipeline Overview

## 1. Objectives
Define the automation flow for build, test, and deployment.

## 2. Pipeline Stages
1. **Build**  
   - Lint, test, and compile.
2. **Test**  
   - Run unit + integration tests.
3. **Package**  
   - Docker build and tag.
4. **Deploy**  
   - Helm upgrade or kubectl apply.

## 3. Tools
- GitHub Actions / Jenkins / GitLab CI
- Docker + Helm + Kubernetes
- SonarQube for code quality
- Snyk for dependency security

## 4. Environments
| Environment | Purpose | Trigger |
|--------------|----------|----------|
| Dev | Feature testing | Push to branch |
| Staging | Integration testing | PR merge |
| Production | Live deployment | Tag release |

## 5. Rollback
Describe rollback procedure and Helm revision rollback command.

## 6. Notifications
CI/CD results sent to Slack channel `#deployments`.
