# 📘 Assignment: Building REST APIs with FastAPI

## 🎯 Objective

Build a small RESTful API using FastAPI to practice designing endpoints, handling request data, and writing asynchronous handlers. Students will implement CRUD-style endpoints, validate input, and test the API using curl or HTTP clients.

## 📝 Tasks

### 🛠️ Core API Mechanics

#### Description
Create a FastAPI application that exposes endpoints to create, read, update, and delete simple "notes". Implement request validation, proper HTTP status codes, and in-memory data storage.

#### Requirements
Completed project should:
- Provide endpoints: GET /notes, GET /notes/{id}, POST /notes, PUT /notes/{id}, DELETE /notes/{id}
- Use Pydantic models for request and response validation
- Return appropriate HTTP status codes (201 for create, 404 for not found, etc.)
- Store data in-memory (dictionary or list) so the app runs without a database
- Include brief inline comments and organize code into functions

Example requests:
```bash
# Create
curl -X POST localhost:8000/notes -H "Content-Type: application/json" -d '{"title":"Todo","content":"Write tests"}'
# Read all
curl localhost:8000/notes
# Read single
curl localhost:8000/notes/1
```

### 🛠️ Enhancements and Deployment

#### Description
Add optional features that improve robustness, usability, and deployment readiness.

#### Requirements
Completed project should include at least two of:
- Query parameters for filtering or pagination (e.g., ?q=term, ?limit=10)
- Basic error handlers for validation and 404 responses
- A simple tests folder with one or two pytest tests hitting endpoints via TestClient
- A small README section on how to run the app (uvicorn command) and run tests
- (Optional) Dockerfile for containerized execution

