# User Registration API

A RESTful API built using **ASP.NET Core Web API** for registering users with proper validation and database integration. This project uses **Entity Framework Core** and **SQL Server** for data persistence.

## 🚀 Features

- Register new users
- Input validation (email format, required fields, password strength)
- Store user data in SQL Server database
- Clean architecture with separation of concerns
- Swagger UI for API testing

## 🛠️ Technologies Used

- ASP.NET Core Web API
- Entity Framework Core
- SQL Server
- Swagger / Swashbuckle
- C#

## 📁 Project Structure

- `Models/` – Defines the `User` entity
- `DTOs/` – Request and response models for clean data handling
- `Controllers/` – API endpoints for user registration
- `Data/` – Database context using EF Core
- `appsettings.json` – Configuration for DB connection string

## 🔄 API Endpoint

| Method | Endpoint              | Description           |
|--------|-----------------------|-----------------------|
| POST   | `/api/users/register` | Register a new user   |

### 📦 Sample JSON Request

```json
{
  "fullName": "John Doe",
  "email": "john.doe@example.com",
  "password": "StrongPass123!"
}
