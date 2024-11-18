Movie Portfolio Platform

Overview

The Movie Portfolio Platform is a Node.js-based application designed to allow users to create, manage, and showcase a portfolio of movies. It provides a user-friendly interface for both administrators and regular users, featuring robust security measures and responsive design.

Features

User Authentication: Secure registration and login system with two-factor authentication (2FA).
Portfolio Management: CRUD (Create, Read, Update, Delete) operations for movie entries.
Role-Based Access Control: Admin and editor roles with different permissions.
API Integration: Fetch movie data from external APIs and display relevant information.
Email Notifications: Nodemailer integration for updates and notifications.
Responsive Design: Clean, mobile-friendly interface.
Technologies Used

Backend: Node.js, Express.js
Database: MongoDB
Frontend: EJS templates, CSS
Authentication: Passport.js, JWT
Email Service: Nodemailer
Environment Management: dotenv
Installation

Clone the repository:
bash

git clone <repository-url>
cd movie-portfolio-123
Install dependencies:
npm install
Create a .env file with the following variables:
makefile

PORT=3000
MONGO_URI=<your-mongodb-connection-string>
JWT_SECRET=<your-jwt-secret>
EMAIL_USER=<your-email>
EMAIL_PASS=<your-email-password>
Start the server:


npm start
Open your browser and navigate to http://localhost:5400.
Folder Structure

css/: Contains CSS files for styling.
models/: Defines database schemas and models.
public/: Static assets like images and JavaScript files.
routes/: API and web routes.
utils/: Helper functions and utilities.
views/: EJS templates for rendering pages.
server.js: Entry point of the application.
.env: Configuration file for environment variables.
Usage

Admin Role
Manage all movie entries.
Assign or revoke editor roles.
Monitor platform activities.

Editor Role
Add and edit movie entries in their assigned portfolios.
View analytics and reports.

Regular Users
View the public movie portfolio.
Search and filter movie entries.

API Endpoints

GET /movies: Fetch all movies.
POST /movies: Add a new movie (Admin/Editor only).
PUT /movies/:id: Update a movie entry (Admin/Editor only).
DELETE /movies/:id: Delete a movie entry (Admin only).
