# 📘 Assignment: Persisting FastAPI Data with SQLite

## 🎯 Objective

Extend a task API to store its data in SQLite instead of keeping it only in memory. Practice creating a database table, using Python's built-in `sqlite3` module, and connecting database operations to FastAPI routes so task data remains available after the application restarts.

## 📝 Tasks

### 🛠️ Create and Explore the SQLite Database

#### Description
Create a SQLite database for the tasks managed by the FastAPI application. Define a table that can store each task's ID, title, and completion status, then add a few records and query them with Python.

#### Requirements
Completed program should:

- Use Python's built-in `sqlite3` module to connect to a database file
- Create a `tasks` table with an integer primary key, a required title, and a completion status
- Insert at least two tasks and retrieve them from the database
- Close database connections when finished with them

### 🛠️ Implement Task Database Operations

#### Description
Write Python functions for the task operations used by the API. Keep database access separate from the route handlers so each operation can be checked independently.

#### Requirements
Completed program should:

- Provide functions to create, list, retrieve, update, and delete tasks
- Use SQL parameters when inserting or updating task data
- Return a clear result when a task ID does not exist
- Demonstrate each operation and confirm that updated data can be queried

### 🛠️ Connect the Database to FastAPI

#### Description
Update the task API so its CRUD routes use the database operations instead of an in-memory collection. Verify that data is still available after stopping and restarting the application.

#### Requirements
Completed program should:

- Initialize the tasks table when the application starts
- Use the database functions in the existing `GET`, `POST`, `PUT`, and `DELETE` task routes
- Preserve the API's existing request validation and appropriate HTTP status codes
- Create a task, restart the application, and confirm the task can still be retrieved
