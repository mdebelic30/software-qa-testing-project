# Login – Test Cases

**Precondition:** A test account exists, unless the test case states otherwise.

TC01 – Successful Login
Positive test

Test Case ID: TC01

Title: Verify successful login with valid credentials

Preconditions: User has an existing account.

Test Data:
- Username: marija123
- Password: Password123
Steps to Execute:
1. Open the login page.
2. Enter a valid username.
3. Enter a valid password.
4. Click the Login button.
Expected Result: The user should be successfully logged in and redirected to the homepage.

Actual Result: To be filled after execution.

Status: Not Run

### TC02 – Verify login with an empty username

**Test Case ID:** TC02

**Title:** Verify that the username field is required

**Test Type:** Negative Testing

**Preconditions:** User is on the login page.

**Test Data:**
- Username: Empty
- Password: `Password123`

**Steps to Execute:**
1. Open the login page.
2. Leave the Username field empty.
3. Enter a valid password.
4. Click the Login button.

**Expected Result:** The application should display a validation message indicating that the username field is required. The user should not be logged in.

**Actual Result:** To be filled after execution.

**Status:** Not Run

### TC03 – Verify username below minimum length

**Test Case ID:** TC03

**Title:** Verify that usernames shorter than 3 characters are rejected

**Test Type:** Negative Testing / Boundary Value Analysis

**Preconditions:** User is on the login page.

**Test Data:**
- Username: `ma`
- Password: `Password123`

**Steps to Execute:**
1. Open the login page.
2. Enter `ma` in the Username field.
3. Enter a valid password.
4. Click the Login button.

**Expected Result:** The application should display a validation message indicating that the username must contain at least 3 characters. The login attempt should be rejected.

**Actual Result:** To be filled after execution.

**Status:** Not Run

### TC04 – Verify username above maximum length

**Test Case ID:** TC04

**Title:** Verify that usernames longer than 20 characters are rejected

**Test Type:** Negative Testing / Boundary Value Analysis

**Preconditions:** User is on the login page.

**Test Data:**
- Username: `marijadebelic12345678`
- Password: `Password123`

**Steps to Execute:**
1. Open the login page.
2. Enter `marijadebelic12345678` in the Username field.
3. Enter a valid password.
4. Click the Login button.

**Expected Result:** The application should display a validation message indicating that the username cannot exceed 20 characters. The login attempt should be rejected.

**Actual Result:** To be filled after execution.

**Status:** Not Run

### TC05 – Verify login with an empty password

**Test Case ID:** TC05

**Title:** Verify that the password field is required

**Test Type:** Negative Testing / Input Validation

**Preconditions:** User is on the login page.

**Test Data:**
- Username: `marija123`
- Password: Empty

**Steps to Execute:**
1. Open the login page.
2. Enter `marija123` in the Username field.
3. Leave the Password field empty.
4. Click the Login button.

**Expected Result:** The application should display a validation message indicating that the password field is required. The user should not be logged in.

**Actual Result:** To be filled after execution.

**Status:** Not Run

### TC06 – Verify password below minimum length

**Test Case ID:** TC06

**Title:** Verify that passwords shorter than 8 characters are rejected

**Test Type:** Negative Testing / Boundary Value Analysis

**Preconditions:** User is on the login page.

**Test Data:**
- Username: `marija123`
- Password: `pass12`

**Steps to Execute:**
1. Open the login page.
2. Enter `marija123` in the Username field.
3. Enter `pass12` in the Password field.
4. Click the Login button.

**Expected Result:** The application should display a validation message indicating that the password must contain at least 8 characters. The login attempt should be rejected.

**Actual Result:** To be filled after execution.

**Status:** Not Run

### TC07 – Verify password above maximum length

**Test Case ID:** TC07

**Title:** Verify that passwords longer than 20 characters are rejected

**Test Type:** Negative Testing / Boundary Value Analysis

**Preconditions:** User is on the login page.

**Test Data:**
- Username: `marija123`
- Password: `Password123456789012`

**Steps to Execute:**
1. Open the login page.
2. Enter `marija123` in the Username field.
3. Enter `Password123456789012` in the Password field.
4. Click the Login button.

**Expected Result:** The application should display a validation message indicating that the password cannot exceed 20 characters. The login attempt should be rejected.

**Actual Result:** To be filled after execution.

**Status:** Not Run
