# API Testing – Authentication

## Purpose

Define checks for an authentication API. Execute these only against a demo, local, or otherwise authorized API.

## Information to collect before testing

- Base URL:
- Endpoint and HTTP method:
- Required headers:
- Request body schema:
- Successful response schema:
- Documented error responses:
- Authentication requirements:

## Planned checks

| ID | Check | Expected result | Status |
|---|---|---|---|
| API-001 | Send a valid login request | Documented success status and response structure | Not Run |
| API-002 | Omit a required field | Documented client-error response and useful validation message | Not Run |
| API-003 | Send an invalid data type | Request is rejected according to the API contract | Not Run |
| API-004 | Use incorrect credentials | Authentication fails with the documented error response | Not Run |
| API-005 | Send an unsupported HTTP method | API returns the documented method-not-allowed behavior, if applicable | Not Run |
| API-006 | Inspect response headers | Content type and relevant headers match the API contract | Not Run |

## Integration checks

- Confirm that the UI sends the expected endpoint, method, headers, and payload.
- Confirm that the UI handles successful API responses correctly.
- Confirm that API validation errors are displayed clearly.
- Confirm that network failures and unexpected responses do not leave the UI in an incorrect state.

## Evidence to capture

Record request method, endpoint, sanitized payload, status code, response body, and execution date. Never commit passwords, access tokens, API keys, or personal data.
