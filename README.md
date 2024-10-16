﻿# Train_Service_Management_System
This is a Train Management System built using Node.js, Express, MongoDB, and Mongoose. The system handles user registration, wallet management, ticket purchasing, station and train management, and more. The application includes authentication and role-based authorization (admin and user) and provides API routes to manage the system efficiently.

Table of Contents:
Features
Technologies
Installation
Environment Variables
API Endpoints
User Authentication
Station Management
Train Management
Wallet Integration
Ticketing System
Error Handling
Postman Collection

Features:
User Registration and Login
Admin and User Roles for different access levels.
Station Management (Add, Update, Retrieve Stations).
Train Management (Add, Update, Retrieve Trains and Schedules).
Wallet Management (Add funds and track transaction history).
Ticketing System (Purchase tickets using wallet balance).
Error Handling with appropriate status codes and error messages.


Technologies:
Node.js: JavaScript runtime for the backend.
Express.js: Fast, unopinionated, minimalist web framework for Node.js.
MongoDB: NoSQL database for storing station, train, ticket, and wallet information.
Mongoose: ODM (Object Data Modeling) library for MongoDB and Node.js.
JWT: Authentication using JSON Web Tokens.

API Endpoints:

User Authentication:
POST /api/user/register
=>Registers a new user.

POST /api/user/login
=>Logs in a user and returns a JWT.

POST /api/user/admin-login
=>Logs in an admin user.

Station Management:
POST /api/station
=>Creates a new station. (Admin only)

PUT /api/station/
=>Updates station details by station ID. (Admin only)

GET /api/station
=>Retrieves a list of all stations.

GET /api/station/
=>Retrieves details of a single station by station ID.

Train Management:
POST /api/train
=>Creates a new train and associated stops. (Admin only)

PUT /api/train/
=>Updates train schedule and stops by train ID. (Admin only)

GET /api/train
=>Retrieves all train schedules.

GET /api/train/
=>Retrieves a single train schedule by train ID.

Wallet Integration:
POST /api/wallet/add
=>Adds funds to the user's wallet.

GET /api/wallet
=>Retrieves the user's wallet balance and transaction history.

Ticketing System:
POST /api/ticket/purchase
=>Purchases a ticket using wallet balance.




