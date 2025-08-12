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

