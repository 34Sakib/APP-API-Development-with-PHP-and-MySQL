# APP-API-Development-with-PHP-and-MySQL

**Task APP API with PHP & MySQL**

This project provides a Task Management API built with PHP and MySQL. It allows users to manage tasks by creating, retrieving, updating, and deleting them through a set of RESTful API endpoints.

**Database Structure**

Database Name: task_api
Table Name: tasks
The tasks table has the following columns:

id: INT, AUTO_INCREMENT, PRIMARY KEY
title: VARCHAR(255), NOT NULL
description: TEXT, NULL
priority: ENUM('low', 'medium', 'high'), DEFAULT 'low'
is_completed: TINYINT(1), DEFAULT 0
created_at: TIMESTAMP, DEFAULT CURRENT_TIMESTAMP
updated_at: TIMESTAMP, ON UPDATE CURRENT_TIMESTAMP

**API Endpoints**

GET /tasks: Retrieve all tasks.
GET /tasks/{id}: Retrieve a specific task by its ID.
POST /tasks: Create a new task. title is required.
PUT /tasks/{id}: Update a task by its ID.
DELETE /tasks/{id}: Delete a task by its ID
