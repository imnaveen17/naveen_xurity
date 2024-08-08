# naveen_xurity

## CRUD Web Application with React, Material-UI, Express, and MongoDB

## Introduction

This is a full-stack CRUD web application built with React for the frontend and Express with MongoDB for the backend. The application features user authentication using JSON Web Tokens (JWT), user registration, and a user list page.

## Features

User Registration: Users can register by providing a username,email id and password.
User Login: Users can log in using their credentials, with JWT-based authentication.
User List Page: Displays a list of all registered users, fetched from the backend.

## Technologies Used

Frontend: React, Material-UI
Backend: Express, MongoDB
Authentication: JSON Web Tokens (JWT)
Password Security: Bcrypt

## Getting Started

**Prerequisites**

Before you begin, ensure you have the following installed:

Node.js (v14 or later)
MongoDB (either locally or a cloud instance)

### Backend Setup

1.**Download the Project Files**

Download the project files and extract them to your local machine.

2.**Navigate to the Backend Directory**

cd your-database-name/backend

3.**Install Dependencies**

npm install

4.**Configure Environment Variables**

Create a .env file in the backend directory with the following content:

MONGODB_URI=mongodb://localhost:27017/your-database-name
JWT_SECRET=/your-database-name

Replace your-database-name with the name of your MongoDB database.
Replace your_jwt_secret with a strong secret key used to sign JWT tokens.

5.**Start the Backend Server**

node server.js

The server will run on http://localhost:5000.

## Frontend Setup

1.**Navigate to the Frontend Directory**

cd client

2.**Install Dependencies**

npm install

npm install @mui/material @emotion/react @emotion/styled (Install Material-UI (MUI):)

3.**Configure Environment Variables**

Create a .env file in the frontend directory with the following content:

REACT_APP_API_URL=http://localhost:5000

4.**Start the Frontend Application**

npm start

The application will run on http://localhost:3000.

## Notes

Database Connection: Ensure MongoDB is running locally or adjust the MONGO_URI if using a remote database like MongoDB Atlas.

Port Conflicts: Ensure that ports 3000 (frontend) and 5000 (backend) are available. If they are in use, you may need to modify the port numbers in your environment variables and application settings.

JWT Secret: Make sure the JWT_SECRET in your .env file is a strong, unique string to ensure secure token signing.
