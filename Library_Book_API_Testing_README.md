# Library Book Management API Testing (Postman)

## Project overview
This beginner API testing project uses Postman Web to test book-related REST API endpoints from FakeRESTAPI.

**Base URL:** `https://fakerestapi.azurewebsites.net/api/v1/Books`

The project demonstrates HTTP methods, request/response validation, JavaScript assertions in Postman, positive and negative testing, and running requests together in Collection Runner.

## Tools and concepts
- Postman Web
- REST API testing
- HTTP methods: GET, POST, PUT, DELETE
- JavaScript test scripts using `pm.test()` and `pm.expect()`
- JSON request and response validation
- Status-code and response-time checks
- Collection Runner

## Test scenarios
| Test Case | Method | Endpoint | Purpose |
|---|---|---|---|
| TC01 - Get All Books | GET | `/api/v1/Books` | Validate list response and required fields |
| TC02 - Get Book by ID | GET | `/api/v1/Books/1` | Validate a single book record |
| TC03 - Add a Book | POST | `/api/v1/Books` | Validate response to a new-book payload |
| TC04 - Update a Book | PUT | `/api/v1/Books/1` | Validate response to an update payload |
| TC05 - Delete a Book | DELETE | `/api/v1/Books/1` | Validate delete response and response time |
| TC06 - Get Non-Existing Book | GET | `/api/v1/Books/999999` | Validate not-found response |

## Execution summary
The project author reported that all six requests passed in Postman's Collection Runner. The scripts described during practice total 22 assertions (4 + 4 + 4 + 4 + 2 + 4). Check the exported collection and current Runner output for authoritative execution details.

## Important limitation
FakeRESTAPI is a sample practice API. Successful POST, PUT, or DELETE responses may simulate an operation or echo submitted data without permanently changing server-side records. Do not claim that books were permanently created, updated, or deleted unless you independently verify persistence.

## How to run
1. Import `Library_Book_API_Testing.postman_collection.json` into Postman.
2. Review each request and its **Scripts → Post-response** assertions.
3. Select **Run collection**.
4. Review passed and failed assertions in Runner results.
5. Save the actual results or screenshots as portfolio evidence.

## Project files
- `Library_Book_API_Testing.postman_collection.json` — export this file from Postman.
- `Library_Book_API_Test_Cases.xlsx` — test scenarios and reported outcomes.
- `Library_Book_API_Testing_README.md` — project overview and instructions.

## Portfolio note
This is a learning project for API testing practice. The execution statuses in the accompanying spreadsheet reflect the author's reported results and have not been independently re-run while preparing these documents.
