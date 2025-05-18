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

## 🖼️ Screenshots
See `setup/screenshots/` for proof-of-concept attack images and successful fixes.

## 📁 Folder Breakdown
| Folder         | Description |
|----------------|-------------|
| `setup/`       | Docker setup and lab configuration |
| `attack_scripts/` | curl payloads used for command-line injection |
| `patched/`     | Secured versions of scripts using prepared statements |
| `report/`      | Assignment write-up and observations |

## 📄 Author
**Aparnaa Mahalaxmi Arulljothi**  
Student ID: A20560995

---

## 🔗 References
- [SEED Labs - SQL Injection](https://seedsecuritylabs.org/Labs_20.04/Web/Web_SQL_Injection/)
- [W3Schools - SQL Injection](https://www.w3schools.com/sql/sql_injection.asp)
