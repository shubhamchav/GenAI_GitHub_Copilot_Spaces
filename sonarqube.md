# 🔹 Basic SonarQube FAQs

## 1. What is SonarQube?

**Answer:**
SonarQube is an open-source platform used for continuous inspection of code quality. It detects:

- Bugs 🐞
- Vulnerabilities 🔐
- Code smells 🧹

It supports multiple languages like Java, JavaScript, Python, C#, etc.

---

## 2. What is a Code Smell?

**Answer:**
A code smell is a maintainability issue that doesn't break functionality but makes code:

- Hard to read
- Hard to maintain
- Error-prone in future

Example: Duplicate code, long methods.

---

## 3. What is a Quality Gate?

**Answer:**
A Quality Gate is a set of conditions that your code must meet before passing analysis.

Example conditions:

- No new bugs
- Code coverage > 80%
- No critical vulnerabilities

If conditions fail → build fails ❌

---

## 4. What is a Quality Profile?

**Answer:**
A Quality Profile defines which rules are applied during analysis.

- Language-specific
- Customizable
- Can enable/disable rules

---

## 5. Difference between Bug, Vulnerability, and Code Smell?

| Type          | Meaning                                  |
|---------------|------------------------------------------|
| Bug           | Logic error causing wrong behavior       |
| Vulnerability | Security risk (e.g., SQL injection)      |
| Code Smell    | Maintainability issue                    |

---

# 🔹 Setup & Architecture Questions

## 6. How does SonarQube work internally?

**Answer:**
SonarQube follows this flow:

1. Code is scanned using SonarScanner
2. Scanner sends data to SonarQube server
3. Server processes and stores results
4. UI displays issues, metrics, and reports

---

## 7. What is SonarScanner?

**Answer:**
A CLI tool that:

- Analyzes source code
- Sends results to SonarQube server

---

## 8. What database does SonarQube use?

**Answer:**
Supports:

- PostgreSQL (recommended)
- MySQL (deprecated since SonarQube 7.9)
- Oracle / SQL Server

---

## 9. Can SonarQube run locally?

**Answer:**
Yes 👍
You can run it locally using:

- ZIP installation
- Docker

Or use the hosted cloud alternative:

- SonarCloud (no self-hosting required)

---

# 🔹 CI/CD Integration

## 10. How to integrate SonarQube with CI/CD?

**Answer:**
Common integrations:

- Jenkins
- GitHub Actions
- GitLab CI

Steps:

1. Install Sonar plugin
2. Configure token
3. Add scan step in pipeline

---

## 11. What is sonar-project.properties?

**Answer:**
A config file that defines:

- Project key
- Source path
- Language
- Server URL
