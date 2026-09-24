# JSONPlaceholder REST API Testing

## Project Overview

This project demonstrates REST API testing using Postman with the JSONPlaceholder Users API.

The project covers CRUD operations, positive and negative test scenarios, response validation, and automated API assertions using Postman scripts.

## Tools & Technologies

- Postman
- JSONPlaceholder REST API
- Microsoft Excel
- JavaScript (Postman test scripts)
- GitHub

## Testing Coverage

The following API operations were tested:

- GET - Retrieve all users
- GET - Retrieve a specific user
- GET - Retrieve a non-existing user
- POST - Create a user
- POST - Create a user with missing fields
- PUT - Update a user
- PATCH - Partially update a user
- DELETE - Delete a user

Additional validations included:

- HTTP status code validation
- Response body validation
- Required field validation
- Data type validation
- Content-Type header validation
- Response time validation
- Positive and negative testing

## Postman Automated Tests

Postman test scripts were implemented to automatically validate API responses.

Automated checks include:

- Status codes
- User IDs
- Required response fields
- Response data types
- Returned user data
- Content-Type
- Response time
- Negative API responses

## Test Results

|     Result       |      Count      |

| Total Test Cases |       12        |
| Passed           |       11        |
| Failed           |       1         |
| Not Executed     |       0         |

### Key Observation

The POST request with missing fields returned `201 Created` instead of the `400 Bad Request` expected by the project test case.

JSONPlaceholder is a mock REST API and does not necessarily enforce these fields as mandatory. Therefore, this result is documented as a mismatch against the project-defined expectation rather than a confirmed defect in JSONPlaceholder.

## What I Learned

Through this project, I gained practical experience in:

- REST API testing using Postman
- Working with GET, POST, PUT, PATCH, and DELETE requests
- Validating HTTP status codes and JSON responses
- Positive and negative API testing
- Writing basic automated assertions using Postman scripts
- Documenting API test cases and test results.

## How to Run the Postman Collection

- Download or clone this repository.
- Open Postman.
- Select Import.
- Import the .postman_collection.json file.
- Open the imported collection.
- Run individual requests to view the API responses and automated test results.




