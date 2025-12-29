# restapi_stg1
A simple Go web server implementing a REST API for creating, retrieving, and deleting users using in-memory storage, JSON, and concurrency-safe access with RWMutex.
🧩 Overview

This repository contains a basic REST API built using Go’s standard net/http package.
The project demonstrates how to build a web server that exposes RESTful endpoints for managing users, without using any external frameworks or databases.

The API stores user data in memory and focuses on explaining core backend concepts such as routing, HTTP methods, JSON handling, concurrency safety, and request/response flow.

🚀 Features

Built using pure Go standard library

RESTful endpoints using HTTP methods:

POST – Create a user

GET – Retrieve a user by ID

DELETE – Delete a user by ID

JSON request and response handling

Thread-safe in-memory storage using sync.RWMutex

Path parameters using Go 1.22+ ServeMux

Beginner-friendly and easy to understand

🛠 Technologies Used

Go (Golang)

net/http

encoding/json

sync.RWMutex

strconv

📡 API Endpoints
Method	Endpoint	Description
GET	/	Health check
POST	/users	Create a new user
GET	/users/{id}	Get user by ID
DELETE	/user/{id}	Delete user by ID
🧪 Testing the API

The API can be tested using:

Postman (recommended for beginners)

curl from the terminal

📌 Purpose

This project is designed for:

Beginners learning Go backend development

Understanding how REST APIs work internally

Learning request handling, JSON parsing, and concurrency control

Practicing API testing using Postman

⚠️ Notes

Data is stored in memory only (no database)

Restarting the server clears all users

Intended for learning and experimentation
