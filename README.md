# Continuous Integration with Docker and GitHub Actions  

## Overview  
This project documents my journey in learning and practicing **Continuous Integration (CI)** using **Docker**, **Docker Compose**, **Makefile**, and **GitHub Actions**.  
I learned how to configure automated pipelines that compile, test, and validate code, ensuring higher quality and reliability in the development process.  

---

<h2 align="center">💻Technologies used</h2>
<p align="center">
  <a href="https://www.docker.com/" target="_blank"><img src="https://img.shields.io/badge/Docker-blue?logo=docker&logoColor=white&labelColor=2b6cb0" alt="Docker Badge"></a>
  <a href="https://docs.docker.com/compose/" target="_blank"><img src="https://img.shields.io/badge/Docker_Compose-0db7ed?logo=docker&logoColor=white&labelColor=1c7ed6" alt="Docker Compose Badge"></a>
  <a href="https://www.gnu.org/software/make/" target="_blank"><img src="https://img.shields.io/badge/Makefile-ef476f?logo=gnu&logoColor=white&labelColor=d6336c" alt="Makefile Badge"></a>
  <a href="https://github.com/features/actions" target="_blank"><img src="https://img.shields.io/badge/GitHub_Actions-2088ff?logo=github&logoColor=white&labelColor=1b6eff" alt="GitHub Actions Badge"></a>
  <a href="https://go.dev/" target="_blank"><img src="https://img.shields.io/badge/Go-00ADD8?logo=go&logoColor=white&labelColor=0a7c99" alt="Go Badge"></a>
</p>

---

## Objectives  
- **Master Continuous Integration (CI):** Understand the complete flow of automated build, test, and validation.  
- **Automation with Docker Compose:** Create isolated and reproducible development environments.  
- **Automated pipeline:** Run tests, linting, and builds without manual intervention.  
- **Security and best practices:** Configure environment variables and secrets securely in GitHub Actions.  
- **Quality control:** Manage Pull Requests and protect the main branch.  

---

## 🧠 Key Learning Areas  

### 🧩 Docker & Docker Compose  
- Building containers for both application and database services.  
- Using **environment variables** to make configurations flexible.  
- Running services with `docker-compose up` and monitoring with `docker-compose logs -f`.  
- Running **automated tests** inside Docker Compose environments.  

### ⚙️ Continuous Integration Workflow  
- Creating **YAML workflows** inside `.github/workflows/`.  
- Defining **jobs** to:  
  - Install dependencies  
  - Run lint and tests  
  - Build Go projects using `go build`  
- Using **GitHub Actions** to automate the entire integration pipeline.  
- Uploading compiled artifacts using `upload-artifact`.  

### 🔒 Security and Configurations  
- Using **GitHub Secrets** to store credentials and sensitive variables securely.  
- Setting up environment variables for integration tests.  
- Protecting the **main branch** with rules that enforce successful test execution before merging.  

### 🛠️ Automation with Makefile  
- Creating simple scripts to automate repetitive tasks.  
- Using commands like `make test`, `make build`, and `make ci` to standardize the development workflow.  
