# Basic SonarQube FAQs

## Question: What is SonarQube?

Answer:
SonarQube is an open-source platform used for continuous inspection of code quality. It detects:

- Bugs
- Vulnerabilities
- Code smells

It supports multiple languages like Java, JavaScript, Python, C#, etc.

Keywords: sonar overview, code quality tool, sonar features

---

## Question: What is a Code Smell?

Answer:
A code smell is a maintainability issue that does not break functionality but makes code:

- Hard to read
- Hard to maintain
- Error-prone in future

Example: Duplicate code, long methods.

Keywords: code smell definition, maintainability issue

---

## Question: What is a Quality Gate?

Answer:
A Quality Gate is a set of conditions that your code must meet before passing analysis.

Example conditions:

- No new bugs
- Code coverage greater than 80%
- No critical vulnerabilities

If conditions fail, the build fails.

Keywords: quality gate sonar, build conditions

---

## Question: What is a Quality Profile?

Answer:
A Quality Profile defines which rules are applied during analysis.

- Language-specific
- Customizable
- Can enable or disable rules

Keywords: quality profile sonar, rules configuration

---

## Question: What is the difference between Bug, Vulnerability, and Code Smell?

Answer:

Type | Meaning
-----|--------
Bug | Logic error causing wrong behavior
Vulnerability | Security risk (for example, SQL injection)
Code Smell | Maintainability issue

Keywords: bug vs vulnerability vs code smell

---

# Setup and Architecture Questions

## Question: How does SonarQube work internally?

Answer:
SonarQube follows this flow:

1. Code is scanned using SonarScanner
2. Scanner sends data to SonarQube server
3. Server processes and stores results
4. UI displays issues, metrics, and reports

Keywords: sonar workflow, sonar architecture

---

## Question: What is SonarScanner?

Answer:
SonarScanner is a CLI tool that:

- Analyzes source code
- Sends results to the SonarQube server

Keywords: sonar scanner, code analysis tool

---

## Question: What database does SonarQube use?

Answer:
SonarQube supports the following databases:

- PostgreSQL (recommended)
- MySQL (deprecated since SonarQube 7.9)
- Oracle
- Microsoft SQL Server

Keywords: sonar database, supported database, sonar db

---

## Question: Can SonarQube run locally?

Answer:
Yes, SonarQube can run locally using:

- ZIP installation
- Docker

You can also use SonarCloud as a hosted alternative.

Keywords: sonar local setup, sonar docker

---

# CI/CD Integration

## Question: How to integrate SonarQube with CI/CD?

Answer:
Common integrations include:

- Jenkins
- GitHub Actions
- GitLab CI

Steps:

1. Install Sonar plugin
2. Configure token
3. Add scan step in pipeline

Keywords: sonar ci cd, sonar integration

---

## Question: What is sonar-project.properties?

Answer:
It is a configuration file that defines:

- Project key
- Source path
- Language
- Server URL

Keywords: sonar config file, sonar properties
