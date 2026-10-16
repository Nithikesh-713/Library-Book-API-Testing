# Library Book Management API Testing using Postman

## Project Overview
This project demonstrates REST API testing using Postman and FakeRESTAPI. It covers HTTP methods, response validation, JSON checks, and automated test assertions written in JavaScript.

## Tools and Technologies
- Postman Web
- REST API Testing
- JavaScript
- JSON
- Microsoft Excel

## API Under Test
**Base URL:** `https://fakerestapi.azurewebsites.net/api/v1/Books`

## Test Scenarios

| Test Case | Method | Endpoint | Purpose |
|---|---|---|---|
| TC01 – Get All Books | GET | `/api/v1/Books` | Validate the list of books and required fields |
| TC02 – Get Book by ID | GET | `/api/v1/Books/1` | Validate a specific book's details |
| TC03 – Add a Book | POST | `/api/v1/Books` | Validate the create-request response |
| TC04 – Update a Book | PUT | `/api/v1/Books/1` | Validate the update-request response |
| TC05 – Delete a Book | DELETE | `/api/v1/Books/1` | Validate the delete response |
| TC06 – Get Non-Existing Book | GET | `/api/v1/Books/999999` | Validate the expected 404 response |

## Validations
- HTTP status codes
- Response time
- JSON response structure
- Book ID, title, and page count
- Submitted or updated values
- Error response for a non-existing book

## Execution Summary
The collection contains six test requests. All test cases passed in my reported Postman Collection Runner execution.

## How to Run
1. Open Postman.
2. Click **Import** and select the exported collection JSON file.
3. Open the collection and review the request URLs and test scripts.
4. Run requests individually or use **Run** to execute the collection.
5. Review the results in the Collection Runner.

## Important Note
FakeRESTAPI is a sample testing service. Successful POST, PUT, and DELETE responses do not necessarily mean data is permanently created, updated, or deleted. This project focuses on request and response validation.

## Skills Demonstrated
- REST API testing
- GET, POST, PUT, and DELETE methods
- Status-code validation
- JSON response validation
- JavaScript assertions
- Negative testing
- Test-case documentation

## Author
Nithikesh H
