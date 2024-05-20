# Spring Project

This project is a Java Spring application designed to manage submissions, documents, requests, employees, submitters, and personal information.

## Functional Requirements

### Submissions Management
- Add new submissions with type, topic, and description.
- Retrieve, update, and delete submissions.
- Associate submissions with documents, requests, and submitters.
### Document Management
- Add documents related to submissions, specifying who issued and accepted the document.
- Retrieve, update, and delete documents.
### Request Management
- Create, retrieve, update, and delete requests associated with submissions.
- Track who requested and accepted the request, along with the request status (is_solved).
### Employee Management
- Add, retrieve, update, and delete employees.
- Link employees to their person details and job post.
### Submitter Management
- Add, retrieve, update, and delete submitters.
- Associate submitters with their person details and status.
### Person Management
- Manage personal information including first name, middle name, and last name.

## System Behaviors

1. Submissions Information
   - Create a submission and link it to documents, requests, and submitters.
   - Update details of a submission.
   - Delete a submission along with associated documents and requests.
   - Retrieve submission details including related documents, requests, and submitters.
2. Documents
   - Upload a document for a specific submission.
   - Update document details such as who issued and accepted it.
   - Delete a document.
   - Retrieve all documents related to a specific submission.
3. Requests
   - Create a request related to a submission.
   - Update request details including the request status.
   - Delete a request.
   - Retrieve all requests related to a specific submission.
4. Employees
   - Add a new employee and link to personal information.
   - Update employee details.
   - Delete an employee.
   - Retrieve employee information including their post and person details.
5. Submitters
   - Add a new submitter and link to personal information.
   - Update submitter details.
   - Delete a submitter.
   - Retrieve submitter information including their status and person details.
6. Persons
   - Add a new person.
   - Update person details.
   - Delete a person.
   - Retrieve person details.

## REST API Endpoints

### Submissions Information
- GET /submissions: Retrieve a list of all submissions.
- GET /submissions/{id}: Retrieve a specific submission by ID.
- POST /submissions: Create a new submission.
- PUT /submissions/{id}: Update a submission by ID.
- DELETE /submissions/{id}: Delete a submission by ID.
### Documents
- GET /submissions/{submissionId}/documents: Retrieve all documents for a specific submission.
- GET /documents/{id}: Retrieve a specific document by ID.
- POST /submissions/{submissionId}/documents: Add a document to a specific submission.
- PUT /documents/{id}: Update a document by ID.
- DELETE /documents/{id}: Delete a document by ID.
### Requests
- GET /submissions/{submissionId}/requests: Retrieve all requests for a specific submission.
- GET /requests/{id}: Retrieve a specific request by ID.
- POST /submissions/{submissionId}/requests: Add a request to a specific submission.
- PUT /requests/{id}: Update a request by ID.
- DELETE /requests/{id}: Delete a request by ID.
### Employees
- GET /employees: Retrieve a list of all employees.
- GET /employees/{id}: Retrieve a specific employee by ID.
- POST /employees: Create a new employee.
- PUT /employees/{id}: Update an employee by ID.
- DELETE /employees/{id}: Delete an employee by ID.
### Submitters
- GET /submitters: Retrieve a list of all submitters.
- GET /submitters/{id}: Retrieve a specific submitter by ID.
- POST /submitters: Create a new submitter.
- PUT /submitters/{id}: Update a submitter by ID.
- DELETE /submitters/{id}: Delete a submitter by ID.
### Persons
- GET /persons: Retrieve a list of all persons.
- GET /persons/{id}: Retrieve a specific person by ID.
- POST /persons: Create a new person.
- PUT /persons/{id}: Update a person by ID.
- DELETE /persons/{id}: Delete a person by ID.
