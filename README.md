📝 Task Manager - Python CLI Application

📌 Overview
This is a simple command-line-based task management application written in Python. It allows users to:

Register with a username and password

Log in using their credentials

Add tasks

View their tasks

Mark tasks as completed

Delete tasks

Key Features
Uses basic file handling (open(...)) for data storage

Does not use any external libraries like os or hashlib

Stores data in plain text files:

users.txt

tasks.txt

📂 File Descriptions
users.txt
Stores registered user credentials.

Format:

pgsql
Copy
Edit
username,password
tasks.txt
Stores all user tasks.

Format:

lua
Copy
Edit
task_id,username,description,status
🔐 Authentication Functions
1. Register
Prompts for username and password

Checks for username duplication

Saves to users.txt if unique

2. Login
Validates username and password

Compares against stored data in users.txt

✅ Task Management Functions
3. Add Task
Prompts for task description

Auto-generates a unique task_id

Appends task to tasks.txt with status Pending

4. View Tasks
Lists all tasks for the logged-in user

Displays ID, description, and status

5. Mark Task as Completed
Prompts for task ID

Updates task status to Completed in tasks.txt

6. Delete Task
Prompts for task ID

Deletes task if it belongs to the user

