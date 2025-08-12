# Asp.net-core-with-mongodb-API
# MongoApiDemo

## Overview

**MongoApiDemo** is a simple RESTful API built with **ASP.NET Core 8** that performs CRUD operations on a MongoDB database. This project demonstrates how to integrate MongoDB with ASP.NET Core using the official MongoDB C# driver.

---

## Features

- Connects to a MongoDB database
- CRUD operations for a `User` entity:
  - Create new users
  - Retrieve all users or by ID
  - Update existing users
  - Delete users by ID
- Clean architecture with service and controller layers
- Configuration via `appsettings.json`

---

## Prerequisites

- [.NET 8 SDK](https://dotnet.microsoft.com/en-us/download/dotnet/8.0)
- [MongoDB Server](https://www.mongodb.com/try/download/community) installed and running on `localhost:27017`
- [Visual Studio 2022](https://visualstudio.microsoft.com/vs/) or any preferred IDE
- [Postman](https://www.postman.com/downloads/) or similar API testing tool (optional)

---

## Getting Started

### Clone the repository

```bash
git clone https://github.com/yourusername/MongoApiDemo.git
cd MongoApiDemo

Setup MongoDB
Make sure your MongoDB server is running:

bash
Copy
Edit
mongod --dbpath "C:\data\db"
Create the folder if it doesn't exist:

bash
Copy
Edit
mkdir C:\data\db
Configure the app
Check and update the connection string in appsettings.json if necessary:

json
Copy
Edit
"MongoDB": {
  "ConnectionString": "mongodb://localhost:27017",
  "DatabaseName": "TestDB",
  "CollectionName": "Users"
}
Run the application
In Visual Studio 2022:

Open the solution

Build the project

Run the app (F5 or Ctrl + F5)

Alternatively, from the command line:

bash
Copy
Edit
dotnet run
API Endpoints
Method	Endpoint	Description
GET	/api/users	Get all users
GET	/api/users/{id}	Get a user by ID
POST	/api/users	Create a new user
PUT	/api/users/{id}	Update a user by ID
DELETE	/api/users/{id}	Delete a user by ID

Example JSON for POST/PUT
json
Copy
Edit
{
  "name": "Alice Smith",
  "email": "alice@example.com"
}
Testing with Postman
Start the application.

Use the endpoints listed above.

Set the header Content-Type: application/json for POST and PUT requests.

Use JSON bodies as shown above.

Technologies Used
ASP.NET Core 8 Web API

MongoDB (NoSQL database)

MongoDB.Driver (Official MongoDB C#/.NET Driver)

Visual Studio 2022

License
This project is licensed under the MIT License. See the LICENSE file for details.

