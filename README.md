🔹 Basic SonarQube FAQs
1. What is SonarQube?

Answer:
SonarQube is an open-source platform used for continuous inspection of code quality. It detects:

Bugs 🐞
Vulnerabilities 🔐
Code smells 🧹

It supports multiple languages like Java, JavaScript, Python, C#, etc.

2. What is a Code Smell?

Answer:
A code smell is a maintainability issue that doesn't break functionality but makes code:

Hard to read
Hard to maintain
Error-prone in future

Example: Duplicate code, long methods.

3. What is a Quality Gate?

Answer:
A Quality Gate is a set of conditions that your code must meet before passing analysis.

Example conditions:

No new bugs
Code coverage > 80%
No critical vulnerabilities

If conditions fail → build fails ❌

4. What is a Quality Profile?

Answer:
A Quality Profile defines which rules are applied during analysis.

Language-specific
Customizable
Can enable/disable rules
5. Difference between Bug, Vulnerability, and Code Smell?
Type	Meaning
Bug	Logic error causing wrong behavior
Vulnerability	Security risk (e.g., SQL injection)
Code Smell	Maintainability issue
🔹 Setup & Architecture Questions
6. How does SonarQube work internally?

Answer:
SonarQube follows this flow:

Code is scanned using SonarScanner
Scanner sends data to SonarQube server
Server processes and stores results
UI displays issues, metrics, and reports
7. What is SonarScanner?

Answer:
A CLI tool that:

Analyzes source code
Sends results to SonarQube server
8. What database does SonarQube use?

Answer:
Supports:

PostgreSQL (recommended)
MySQL (deprecated)
Oracle / SQL Server
9. Can SonarQube run locally?

Answer:
Yes 👍
You can run it using:

ZIP installation
Docker
Cloud (SonarCloud)

🔹 CI/CD Integration
10. How to integrate SonarQube with CI/CD?

Answer:
Common integrations:

Jenkins
GitHub Actions
GitLab CI

Steps:

Install Sonar plugin
Configure token
Add scan step in pipeline
11. What is sonar-project.properties?

Answer:
A config file that defines:

Project key
Source path
Language
Server URL
