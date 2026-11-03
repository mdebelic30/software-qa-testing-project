# Login – Test Cases

**Precondition:** A test account exists, unless the test case states otherwise.

| ID | Scenario | Test data / action | Expected result | Status |
|---|---|---|---|---|
| LOGIN-001 | Login with valid credentials | Enter a registered username and correct password | User is authenticated and redirected to the expected page | Not Run |
| LOGIN-002 | Empty username | Leave username empty; enter a valid password | Required-field validation is displayed; request is not submitted if client-side validation is required | Not Run |
| LOGIN-003 | Empty password | Enter username; leave password empty | Required-field validation is displayed | Not Run |
| LOGIN-004 | Both fields empty | Submit without entering data | Required-field validation is displayed for both fields | Not Run |
| LOGIN-005 | Incorrect password | Enter a valid username and incorrect password | Login is rejected and an appropriate error is displayed | Not Run |
| LOGIN-006 | Unknown username | Enter an unregistered username and a password | Login is rejected without exposing sensitive account information | Not Run |
| LOGIN-007 | Leading/trailing spaces | Enter credentials with surrounding spaces | Behavior matches the documented input-handling rules | Not Run |
| LOGIN-008 | Password visibility control | Toggle password visibility | Password visibility changes without altering the entered value | Not Run |
| LOGIN-009 | Submit using Enter key | Fill credentials and press Enter | Form submits once and handles the response correctly | Not Run |
| LOGIN-010 | Repeated submission | Submit the form repeatedly in quick succession | Application handles repeated requests consistently and does not create an incorrect state | Not Run |

## Execution notes

For each test, record:
- Actual result
- Pass / Fail / Blocked
- Date and environment
- Evidence (screenshot, request/response, or log), where appropriate
