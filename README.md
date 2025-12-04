# Secure PKI-Based 2FA Microservice

This project implements a secure, containerized microservice for TOTP (Time-based One-Time Password) two-factor authentication. It demonstrates enterprise-grade security practices using RSA 4096-bit encryption, digital signatures, and Docker.

## 🚀 Features
- **RSA-OAEP Decryption:** Securely receives and decrypts sensitive seeds.
- **TOTP Generation:** Generates RFC-compliant 2FA codes.
- **Dockerized:** Runs as a secure microservice with persistent volumes.
- **Cron Job:** Logs 2FA codes every minute for auditing (UTC timezone).
- **Security:** Keys are managed via PKI; strict validation on all inputs.

## 🛠️ Tech Stack
- **Language:** Python 3.11
- **Framework:** FastAPI
- **Cryptography:** `cryptography` (RSA-PSS, RSA-OAEP), `pyotp`
- **DevOps:** Docker, Docker Compose, Linux Cron

## ⚙️ Setup & Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/sunil-polupalli/pki-2fa-service.git
   cd pki-2fa-service