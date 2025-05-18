# SQL Injection Attack Lab (SEED Labs)

This project demonstrates SQL Injection vulnerabilities and exploitation techniques using a custom vulnerable web application built for SEED Labs.

## 🔍 Objective
- Understand how SQL injection works
- Perform attacks via web interface and command-line tools
- Modify database values using injection payloads
- Implement countermeasures using prepared statements

## 🧰 Tools Used
- MySQL
- PHP
- Docker
- cURL
- SEED Ubuntu 20.04 VM

## 📌 Key Attacks Performed
- **Bypass Login:** Used `' OR '1'='1` style payloads via browser and curl
- **Data Extraction:** Retrieved employee details using crafted SQL
- **Data Tampering:** Updated salary/password using injection
- **Command Line Injection:** Used encoded SQL in curl requests
- **Defense:** Replaced vulnerable SQL with prepared statements

## 🛡️ Mitigation
- Used PHP's `prepare()` and `bind_param()` methods to eliminate SQL injection risks.


