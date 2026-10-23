# 📘 Assignment: Building REST APIs with FastAPI

## 🎯 Objective

Build a small REST API with FastAPI to manage a collection of tasks. You will practice defining routes, implementing CRUD operations, validating request data, and using HTTP status codes and the interactive API documentation.

## 📝 Tasks

### 🛠️ Create the FastAPI App and Read Routes

#### Description
Create a FastAPI application for managing tasks. Each task should have an integer ID, a title, and a completion status. Store tasks in memory so the API can be completed without setting up a database.

#### Requirements
Completed program should:

- Start a FastAPI application that can be run with Uvicorn
- Define a `GET /tasks` route that returns all tasks as JSON
- Define a `GET /tasks/{task_id}` route that returns the matching task
- Return HTTP 404 when the requested task ID does not exist


### 🛠️ Implement Task CRUD Operations

#### Description
Add routes that let API users create, update, and delete tasks. Use the task ID in the URL to identify which task should be changed or removed.

#### Requirements
Completed program should:

- Define `POST /tasks` to create a task and return its assigned ID
- Define `PUT /tasks/{task_id}` to update an existing task
- Define `DELETE /tasks/{task_id}` to remove an existing task
- Return HTTP 404 when an update or delete request targets a missing task
- Verify that creating, reading, updating, and deleting tasks works through the API


### 🛠️ Validate Requests and Explore the API

#### Description
Use a Pydantic model to describe task data and let FastAPI validate incoming requests. Check the interactive API documentation and try both valid and invalid requests.

#### Requirements
Completed program should:

- Define a Pydantic model for task input, requiring a non-empty title and a boolean completion status
- Use the model for create and update request bodies
- Return an appropriate success status for creating a task and for deleting a task
- Open FastAPI's `/docs` page and use it to try each route
- Confirm that invalid request data is rejected with a validation error
