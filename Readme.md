# Task Management REST API

## Project Overview
A RESTful API for managing users, projects, and tasks.

## Technologies Used
- Node.js
- Express.js
- MySQL
- MongoDB
- Mongoose
- JWT Authentication
- bcryptjs

## Database Design
- MySQL stores user and project information.
- MongoDB stores task information.
- Each task stores its project ID and owner ID.

## Installation

1. Clone the repository.
2. Install dependencies:

   `npm install`

3. Create a `.env` file using `.env.example`.
4. Configure MySQL and create the task_management database.
5. Configure MongoDB and update MONGO_URI.
6. Start the application:

   `npm run dev`

## Authentication APIs
- POST /api/auth/register
- POST /api/auth/login
- GET /api/auth/me
- PUT /api/auth/profile

## Project APIs
- POST /api/projects
- GET /api/projects
- GET /api/projects/:id
- PUT /api/projects/:id
- DELETE /api/projects/:id

## Task APIs
- POST /api/tasks
- GET /api/tasks
- GET /api/tasks/:id
- PUT /api/tasks/:id
- DELETE /api/tasks/:id

## Dashboard API
- GET /api/dashboard

## Task Status
- todo
- in_progress
- completed

## Task Priority
- low
- medium
- high

## Filtering and Pagination
Example:

`GET /api/tasks?page=1&limit=10&status=todo&priority=high`

## Authentication
Protected APIs require a JWT Bearer Token.

## Testing
APIs can be tested using Postman or Thunder Client.
