# To-Do Application API

This is a RESTful API for a To-Do application, built using Node.js, Express, and MongoDB. The application supports user authentication using jsonwebtoken and  supports crud operation for both users and tasks.

## Features
- User authentication using json web token(Register/Login)
- Create, Read, Update, and Delete  operations for tasks
- Secure API endpoints using JWT authentication
  
Setup Instructions

Follow these steps to set up and run the To-Do Application API:

Initialize the Node.js Server:

npm init -y

This will create a package.json file to manage dependencies.

Install Necessary Libraries:
Install the required dependencies using:

npm install express mongoose dotenv bcrypt jsonwebtoken nodemon

Configure Environment Variables:

Create a .env file in the root directory.

Add the following variables:

PORT=5000
MONGO_URL=your_mongodb_connection_string
JWT_SECRET=your_secret_key

Set Up Git Ignore:

Create a .gitignore file.

Add files that should not be pushed to the repository:

node_modules/
.env

Setup Database Models:

Create a models folder.

Define the User and Task schemas in separate files.

Create API Routes:

Inside the routes folder, create separate route files for:

Authentication (register, login)

User-related operations

Task-related operations

Implement Authentication Middleware:

Create a middleware for verifying JWT tokens.

Ensure protected routes require authentication.

Test APIs Using Thunder Client or Postman:

Use tools like Thunder Client or Postman to test API endpoints.

Check if tasks can be created, updated, deleted, and retrieved.

Running the Application

Start the server using Nodemon for automatic restarts:

npx nodemon index.js

Or manually run:

node index.js

The API will be available at:

http://localhost:5000

API Endpoints

Authentication

POST /api/auth/register – Register a new user.

POST /api/auth/login – Authenticate and get a token.

Tasks

POST /api/tasks – Create a new task (Authenticated).

GET /api/tasks – Get all tasks (Authenticated).

GET /api/tasks/completed – Get completed tasks (Authenticated).

PUT /api/tasks/:id – Update a task (Authenticated).

DELETE /api/tasks/:id – Delete a task (Authenticated).
