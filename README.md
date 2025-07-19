# 🚀 PHP Yii2 CI/CD Deployment - Part 3
<img width="1919" height="1033" alt="image" src="https://github.com/user-attachments/assets/51244901-83b4-4620-b227-f473a7c8588f" />
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/bfa186c5-5160-4492-8a3d-3e967e2b1e54" />
<img width="1919" height="1031" alt="image" src="https://github.com/user-attachments/assets/ba0c9e47-164b-485a-97fd-a170d87d512b" />
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/cfba8eb3-b6f2-4b96-afe3-d306b0b1dfa5" />



This project demonstrates a **CI/CD pipeline for a PHP Yii2 application** using **Jenkins**, **Docker Compose**, and **MySQL**, with **secure credential injection** for database access. The application is containerized and deployed in a local development environment.

---

## 📁 Project Structure



---

## ⚙️ Technologies Used

- PHP (Yii2 Framework)
- MySQL (via Docker)
- Docker & Docker Compose
- Jenkins (Declarative Pipeline)
- GitHub (Source Code Management)
- Jenkins Credentials (Username & Password)

---

## 📌 Features

✅ Secure `.env` generation via Jenkins  
✅ Dynamic injection of DB credentials using Jenkins credentials store  
✅ Docker Compose setup for PHP & MySQL  
✅ Automated container build and up  
✅ Retry mechanism to wait for DB readiness  
✅ DB migration (optional/skipped in current version)  
✅ Mock Unit Test step  
✅ Apache server container startup check  
✅ Logs and status printout for visibility  

---

## 🛠️ Setup Instructions

### 1. 🔐 Jenkins Credential Setup

In Jenkins UI:

- Go to **Manage Jenkins → Credentials → Global → Add Credentials**
- Choose **Username with password**
  - **ID:** `DB_USER`
  - **Username:** your MySQL username (e.g., `root`)
  - **Password:** your MySQL password

---

### 2. 🐳 Docker Requirements

Install:

- Docker: https://docs.docker.com/get-docker/
- Docker Compose: https://docs.docker.com/compose/install/

---

### 3. 📦 Run Locally (Optional Manual Run)

```bash
docker-compose build
docker-compose up -d
