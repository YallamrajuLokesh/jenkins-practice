# jenkins-practice
# Jenkins CI/CD Practice Repository 🤖

This repository is dedicated to practicing Continuous Integration and Continuous Deployment (CI/CD) workflows using Jenkins. It serves as a sandbox for SDET automation concepts.

## 🎯 Project Objectives
* Understand Declarative Pipeline syntax (Groovy).
* Manage Windows-based build environments (`bat` commands).
* Automate job triggers using SCM Polling and Cron scheduling.
* Generate and archive test execution artifacts.

## 🛠️ Pipeline Architecture
The `Jenkinsfile` in this project executes the following stages:
1. **Build App:** Compiles the initial code structure.
2. **Run Tests:** Executes the automated test suite (simulated Pytest environment).
3. **Deploy:** Pushes to the staging environment (conditional on test success).

## 📊 Status
* **Trigger Mechanism:** SCM Polling (`* * * * *`)
* **Current State:** Actively testing Git-to-Jenkins webhooks and polling.
