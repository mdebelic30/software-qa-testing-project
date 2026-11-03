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

**Actual Result:** The application displayed the message: "Congratulations student. You successfully logged in!"

**Status:** Passed

**Execution Notes:** Login was successful using valid demo credentials on Practice Test Automation.

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

**Actual Result:** The application displayed the error message: "Your username is invalid!"

**Status:** Passed

**Execution Notes:** Login was rejected when the username field was left empty.

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

**Actual Result:** The application displayed the error message: "Your username is invalid!"

**Status:** Passed

**Execution Notes:** Login was rejected when a username shorter than the minimum allowed length (3 characters) was entered.

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

**Actual Result:** The application displayed the error message: "invalid username".

**Status:** Passed

**Execution Notes:** Login was rejected when a username exceeding the maximum allowed length (20 characters) was entered.

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

**Actual Result:** The application displayed the error message: "Your password is invalid!"

**Status:** Passed

**Execution Notes:** Login was rejected when the password field was left empty.

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

**Actual Result:** The application displayed the error message: "invalid password".

**Status:** Passed

**Execution Notes:** Login was rejected when a password shorter than the minimum allowed length (8 characters) was entered.

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

**Actual Result:** The application displayed the error message: "invalid password".

**Status:** Passed

**Execution Notes:** Login was rejected when a password exceeding the maximum allowed length (20 characters) was entered.

### TC08 – Verify login with invalid credentials

**Test Case ID:** TC08

**Title:** Verify that login is rejected when invalid credentials are entered

**Test Type:** Negative Testing / Authentication Testing

**Preconditions:** User is on the login page. The test username does not belong to an existing account.

**Test Data:**
- Username: `wronguser123`
- Password: `WrongPass123`

**Steps to Execute:**
1. Open the login page.
2. Enter `wronguser123` in the Username field.
3. Enter `WrongPass123` in the Password field.
4. Click the Login button.

**Actual Result:** The application displayed the error message: "invalid password".

**Status:** Passed

**Execution Notes:** Login was rejected when an incorrect password was entered for a valid username.

### TC09 – Verify login with both fields empty

**Test Case ID:** TC09

**Title:** Verify that login is rejected when both username and password fields are empty

**Test Type:** Negative Testing / Input Validation

**Preconditions:** User is on the login page.

**Test Data:**
- Username: Empty
- Password: Empty

**Steps to Execute:**
1. Open the login page.
2. Leave the Username field empty.
3. Leave the Password field empty.
4. Click the Login button.

**Actual Result:** The application displayed the error message: "Your username is invalid!"

**Status:** Passed

**Execution Notes:** Login was rejected when both username and password fields were left empty. However, the application displayed only a username-related error message.

### TC10 – Verify login with different username letter casing

**Test Case ID:** TC10

**Title:** Verify that username login is case-insensitive

**Test Type:** Functional Testing / Input Validation

**Preconditions:**
- User has an existing account.
- The registered username is `marija123`.
- The application treats usernames as case-insensitive.

**Test Data:**
- Username: `MARija123`
- Password: `Password123`

**Steps to Execute:**
1. Open the login page.
2. Enter `MARija123` in the Username field.
3. Enter the correct password.
4. Click the Login button.

**Actual Result:** The application displayed the error message: "username is invalid".

**Status:** Failed

**Execution Notes:** Login failed when the valid username "student" was entered in uppercase as "STUDENT". The application appears to treat usernames as case-sensitive.
