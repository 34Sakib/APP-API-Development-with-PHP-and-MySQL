# APP-API-Development-with-PHP-and-MySQL

Task APP API with PHP & MySQL

This API is built using PHP and MySQL to manage tasks. It supports creating, retrieving, updating, and deleting tasks.

Database Structure

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
API Endpoints

GET /tasks: Retrieve all tasks.
GET /tasks/{id}: Retrieve a specific task by ID.
POST /tasks: Create a new task. title is required.
PUT /tasks/{id}: Update a task by ID.
DELETE /tasks/{id}: Delete a task by ID.
Installation

Clone the repository:
git clone https://github.com/yourusername/task-api.git
Set up the MySQL database and configure your credentials in config.php.
Run the PHP server:
php -S localhost:8000
License

MIT License
