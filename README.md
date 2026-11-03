# Software QA & Testing Portfolio

A hands-on Software Quality Assurance portfolio demonstrating practical experience in manual testing, API testing, test case design, bug reporting, and automated response validation using Postman and JavaScript.

## Project Overview

This repository contains QA documentation and practical testing exercises performed on publicly available demo applications and APIs.

The main objective is to demonstrate a structured approach to software testing, including test planning, test execution, validation of expected results, and clear defect documentation.

## Project Scope

### 1. Manual Testing – Login Functionality

**Application:** [Practice Test Automation – Login Page](https://practicetestautomation.com/practice-test-login/)

Testing activities include:
- Positive and negative testing
- Login validation
- Empty field validation
- Boundary value analysis
- Invalid credentials testing
- Username case sensitivity testing

**Execution Results:**
- 10 test cases executed
- 9 Passed
- 1 Failed against the assumed expected behavior

The failed test concerns username case sensitivity. The expected behavior requires clarification before confirming a product defect.

### 2. API Testing – JSONPlaceholder

**API:** [JSONPlaceholder](https://jsonplaceholder.typicode.com/)

**Tool:** Postman  
**Scripting Language:** JavaScript

HTTP methods tested:
- GET – Retrieve resources
- POST – Create resources
- PUT – Update resources
- PATCH – Partially update resources
- DELETE – Delete resources

Additional testing activities:
- Positive and negative API testing
- HTTP status code validation
- JSON response validation
- Automated assertions using JavaScript

**Execution Results:**
- 6 API test scenarios executed
- 22 automated assertions
- 22 Passed
- 0 Failed

*Note: JSONPlaceholder is a simulated REST API. POST, PUT, PATCH, and DELETE operations return simulated responses and do not permanently modify the underlying database.*

## Testing Techniques

- Functional Testing
- Positive Testing
- Negative Testing
- Boundary Value Analysis
- Input Validation
- Manual API Testing
- Automated API Response Validation
- HTTP Status Code Validation
- JSON Response Validation
- Bug Identification and Reporting

## Tools & Technologies

| Tool / Technology | Purpose |
|---|---|
| Postman | API testing and request execution |
| JavaScript | Automated API test assertions |
| Git | Version control |
| GitHub | Project hosting and documentation |
| Git Bash | Command-line operations |
| Markdown | QA documentation |

## Repository Structure

```text
software-qa-testing-project/
│
├── README.md
│
├── Test-Plan/
│   └── test-plan.md
│
├── Test-Cases/
│   ├── login-test-cases.md
│   └── registration-test-cases.md
│
├── Bug-Reports/
│   ├── bug-report-template.md
│   └── BR-001-username-case-sensitivity.md
│
├── API-Testing/
│   ├── api-test-plan.md
│   └── api-test-results.md
│
└── Test-Results/
    └── test-summary-template.md
```

## Test Documentation

- [Test Plan](Test-Plan/test-plan.md)
- [Login Test Cases](Test-Cases/login-test-cases.md)
- [Registration Test Cases](Test-Cases/registration-test-cases.md)
- [Bug Report – BR-001](Bug-Reports/BR-001-username-case-sensitivity.md)
- [API Test Plan](API-Testing/api-test-plan.md)
- [API Test Execution Results](API-Testing/api-test-results.md)

## Key Learning Outcomes

Through this project, I have gained practical experience in:

- Designing and executing test cases.
- Identifying and documenting unexpected application behavior.
- Performing positive and negative testing.
- Testing REST API endpoints using Postman.
- Writing JavaScript assertions for automated API validation.
- Analyzing HTTP responses and status codes.
- Managing QA documentation using Git and GitHub.

## Author

**Marija Debelić**

BSc in Web & Mobile Computing

[GitHub Profile](https://github.com/mdebelic30)  
[LinkedIn Profile](https://www.linkedin.com/in/marija-debeli%C4%87-0330b3251)

---

*This portfolio is an ongoing learning project. Additional test scenarios and testing activities will be added as the project develops.*