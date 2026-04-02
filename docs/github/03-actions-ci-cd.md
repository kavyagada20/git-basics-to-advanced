# ⚙️ GitHub Actions & CI/CD

---

## 📌 Overview

GitHub Actions is a powerful tool that enables **automation of workflows** directly inside your repository.

It is commonly used to implement **CI/CD (Continuous Integration / Continuous Deployment)**.

---

## 🔧 What is CI/CD?

### 🔹 Continuous Integration (CI)
Automatically builds and tests code when changes are pushed.

### 🔹 Continuous Deployment (CD)
Automatically deploys code after successful tests.

---

## 🚀 What is GitHub Actions?

GitHub Actions allows you to:
- Automate workflows
- Run tests
- Build applications
- Deploy projects

---

## 📂 Workflow Location

Workflows are stored in:

```bash
.github/workflows/
🧪 Basic Workflow Example

Create a file:

.github/workflows/ci.yml
📄 Example: Node.js CI Workflow
name: CI Pipeline

on:
  push:
    branches: [ main ]
  pull_request:
    branches: [ main ]

jobs:
  build:
    runs-on: ubuntu-latest

    steps:
      - name: Checkout code
        uses: actions/checkout@v3

      - name: Setup Node.js
        uses: actions/setup-node@v3
        with:
          node-version: '18'

      - name: Install dependencies
        run: npm install

      - name: Run tests
        run: npm test
🔄 Workflow Trigger Events

Common triggers:

push
pull_request
schedule
workflow_dispatch
⚙️ Key Components
🔹 Workflow

Automation defined in YAML file

🔹 Job

A set of steps executed on a runner

🔹 Step

Individual task inside a job

🔹 Action

Reusable unit of code

🚀 CI/CD Pipeline Flow
Code Push → Build → Test → Deploy
🌐 Common Use Cases
Run automated tests
Lint code
Build applications
Deploy to servers/cloud
🧠 Best Practices
Keep workflows simple
Use caching for faster builds
Separate jobs logically
Use secrets for sensitive data
🔐 GitHub Secrets

Store sensitive data like:

API keys
Tokens

Access via:

${{ secrets.SECRET_NAME }}
⚠️ Common Mistakes
Hardcoding secrets
Overcomplicated workflows
Not testing workflows locally
🎯 Summary
GitHub Actions automates workflows
Enables CI/CD pipelines
Improves development efficiency
➡️ Next Step

Continue to:

👉 04-collaboration.md