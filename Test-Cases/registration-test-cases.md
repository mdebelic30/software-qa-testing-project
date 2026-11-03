# Registration – Test Cases

**Precondition:** Registration page is available. Confirm the actual validation rules before execution.

| ID | Scenario | Test data / action | Expected result | Status |
|---|---|---|---|---|
| REG-001 | Register with valid data | Complete all required fields with valid, unused data | Account is created and success feedback is displayed | Not Run |
| REG-002 | All fields empty | Submit the form without entering data | Required-field validation is displayed | Not Run |
| REG-003 | Missing username | Leave username empty and complete other fields | Username validation is displayed | Not Run |
| REG-004 | Missing password | Leave password empty and complete other fields | Password validation is displayed | Not Run |
| REG-005 | Password below minimum length | Enter a password one character shorter than the stated minimum | Input is rejected with a clear validation message | Not Run |
| REG-006 | Password at minimum length | Enter a password exactly at the stated minimum | Input is accepted if all other rules are met | Not Run |
| REG-007 | Password above maximum length | Enter a password one character longer than the stated maximum, if a maximum exists | Input is handled according to the documented limit | Not Run |
| REG-008 | Existing username/email | Attempt registration with an already registered identifier | Duplicate registration is rejected with an appropriate message | Not Run |
| REG-009 | Invalid email format | Enter malformed email data | Email validation is displayed | Not Run |
| REG-010 | Whitespace-only input | Enter spaces in required text fields | Whitespace is not incorrectly accepted as valid content | Not Run |

## Boundary value analysis

Do not assume a five-character password rule. First identify the application's actual minimum and maximum limits. Then test:
- One value below the minimum
- The exact minimum
- One value above the minimum
- The exact maximum, if defined
- One value above the maximum
