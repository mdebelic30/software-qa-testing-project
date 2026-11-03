# API Testing – Authentication

# API Testing – Test Execution Results

## 1. Project Overview

**API:** JSONPlaceholder  
**Base URL:** https://jsonplaceholder.typicode.com  
**Tool:** Postman  
**Scripting Language:** JavaScript  
**Testing Type:** Manual API Testing and Automated Response Validation

## 2. Test Execution Summary

A total of 6 API test scenarios were executed using Postman.

| Test Scenario | HTTP Method | Expected Status | Actual Status | Result |
|---|---|---|---|---|
| Retrieve existing post | GET | 200 | 200 | Passed |
| Retrieve non-existing post | GET | 404 | 404 | Passed |
| Create new post | POST | 201 | 201 | Passed |
| Update existing post | PUT | 200 | 200 | Passed |
| Partially update post | PATCH | 200 | 200 | Passed |
| Delete post | DELETE | 200 | 200 | Passed |

## 3. Detailed Test Results

### TC-API-01 – Retrieve Existing Post

- **Method:** GET
- **Endpoint:** `/posts/1`
- **Expected Result:** HTTP 200 OK and valid JSON response.
- **Validations:**
  - Status code is 200.
  - Response contains correct userId.
  - Response contains correct post ID.
  - Title is not empty.
- **Result:** Passed (4/4 assertions).

### TC-API-02 – Retrieve Non-Existing Post

- **Method:** GET
- **Endpoint:** `/posts/9999`
- **Expected Result:** HTTP 404 Not Found.
- **Validations:**
  - Status code is 404.
  - Response does not contain post data.
- **Result:** Passed (2/2 assertions).

### TC-API-03 – Create New Post

- **Method:** POST
- **Endpoint:** `/posts`
- **Expected Result:** HTTP 201 Created.
- **Test Data:**
  - Title: My first API test
  - Body: Learning API testing with Postman
  - User ID: 1
- **Validations:**
  - Status code is 201.
  - Response contains correct title.
  - Response contains correct userId.
  - Response contains generated ID.
- **Result:** Passed (4/4 assertions).

### TC-API-04 – Update Existing Post

- **Method:** PUT
- **Endpoint:** `/posts/1`
- **Expected Result:** HTTP 200 OK and updated resource.
- **Validations:**
  - Status code is 200.
  - Response contains updated title.
  - Response contains updated body.
  - Response contains correct post ID.
  - Response contains correct userId.
- **Result:** Passed (5/5 assertions).

### TC-API-05 – Partially Update Post

- **Method:** PATCH
- **Endpoint:** `/posts/1`
- **Expected Result:** HTTP 200 OK and updated title.
- **Validations:**
  - Status code is 200.
  - Title is updated.
  - Post ID remains unchanged.
  - User ID remains unchanged.
  - Body remains unchanged.
- **Result:** Passed (5/5 assertions).

### TC-API-06 – Delete Post

- **Method:** DELETE
- **Endpoint:** `/posts/1`
- **Expected Result:** HTTP 200 OK and empty response body.
- **Validations:**
  - Status code is 200.
  - Response body is empty.
- **Result:** Passed (2/2 assertions).

## 4. Overall Results

| Metric | Result |
|---|---:|
| Total test scenarios | 6 |
| Total assertions | 22 |
| Passed assertions | 22 |
| Failed assertions | 0 |
| Pass rate | 100% |

## 5. Testing Conclusion

All executed API test scenarios passed successfully.

The testing covered:
- HTTP methods: GET, POST, PUT, PATCH and DELETE.
- Positive and negative API testing.
- HTTP status code validation.
- JSON response validation.
- Automated assertions using JavaScript in Postman.

**Note:** JSONPlaceholder is a fake online REST API. POST, PUT, PATCH and DELETE operations simulate server responses and do not permanently modify the underlying database.

## 6. Tools and Technologies

- Postman
- JavaScript
- REST API
- JSON
- Git
- GitHub