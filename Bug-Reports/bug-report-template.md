# Bug Report Template

# BR-001 – Username Case Sensitivity

**Bug ID:** BR-001

**Title:** Login rejects username entered in uppercase

**Related Test Case:** TC10

**Environment:** Practice Test Automation – Login Page  
**URL:** https://practicetestautomation.com/practice-test-login/

**Preconditions:**
- A valid user account exists.
- Valid credentials are available.

**Steps to Reproduce:**
1. Open the login page.
2. Enter `STUDENT` in the Username field.
3. Enter `Password123` in the Password field.
4. Click Submit.

**Test Data:**
- Username: `STUDENT`
- Password: `Password123`

**Expected Result:**  
The application should accept the username regardless of letter case, if usernames are intended to be case-insensitive.

**Actual Result:**  
The application displayed the error message: "username is invalid".

**Status:** Needs Clarification

**Severity:** Not determined

**Priority:** Not determined

**Notes:**  
The application appears to treat usernames as case-sensitive. Further clarification of the expected username validation behavior is required before classifying this as a confirmed defect.