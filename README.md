ReqRes API Testing – Phase 1

API testing project using Postman to validate the functionality, reliability, and error handling of the ReqRes API.

This project demonstrates common QA practices including:
	•	Authentication testing
	•	Happy path validation
	•	Negative testing
	•	API response validation
	•	Status code verification

⸻

Tools Used
	•	Postman (API testing)
	•	GitHub (version control)
	•	ReqRes API (test API)

⸻

The Postman collection is organized into logical test categories:
    Authentication
    Happy Path
    Sad Path

⸻
## ** Authentication Tests **
Tests for login functionality and credential validation.

POST login request that returns an authentication token.

Validation performed:
- Status code is 200
- Token exists in response

Negative Test - Missing Password

Login request missing the password field.

Validations performed:
- Status code is 400
- Proper error message is returned

## ** Happy Path Tests **

GET Users - Page 1
Retrive the first page of users.

GET Users - Page 2
Retrive the second page of users.

GET Single User
Fetch a specific user.

POST Create User
Create a new user record.

PUT Update a User
Update a user completely.

PATCH Partial Update
Update only specific user field.

DELETE Remove a User
Delete an existing an user.

Typical validations in these include:
- Status code validation
- Response structure validation
- Response time checks
- Data presence verifications

## ** Negative (SAD Path) Tests **

GET Invalid Page
Request a page that does not exists.

GET Invalid User ID
Request a user ID that does not exists.

POST Missing Field
Attempt to create a user with missing required data.

These tests verify:
- Proper error responses
- Correct HTTP status codes
- API error handling behaviour

## Test Coverage

- Authentication testing
- CRUD API operations
- Happy Path scenarios
- Negative testing
- API response validation
- Error handling validation