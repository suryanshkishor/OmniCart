# 🛒 OmniCart: RESTful E-Commerce Inventory API

## 📌 Overview
OmniCart is a robust, highly scalable RESTful API built with C# and the ASP.NET Core Web API framework. It is designed to manage the backend inventory logic for a modern e-commerce platform. This project demonstrates enterprise-level software engineering principles, including the Repository Pattern, Dependency Injection, and asynchronous data operations.

## 🚀 Key Features
* **Full CRUD Operations:** Complete endpoints to Create, Read, Update, and Delete product inventory records securely.
* **Asynchronous Processing:** Utilizes `async/await` patterns throughout the controller and service layers to handle high-volume traffic without blocking server threads.
* **Data Validation:** Implements strict Data Annotations to ensure data integrity (e.g., preventing negative inventory counts or invalid pricing) before data reaches the persistence layer.
* **In-Memory Persistence:** (Configured for testing) Uses Entity Framework Core with an In-Memory Database to allow for rapid deployment and testing without requiring external database setups.

## 🛠️ Tech Stack
* **Language:** C# 12
* **Framework:** ASP.NET Core 8 Web API
* **ORM:** Entity Framework Core (EF Core)
* **API Testing:** Swagger UI (Swashbuckle)

## ⚙️ Core Architecture (The Repository Pattern)
The application architecture is strictly decoupled to ensure maintainability:
1.  **Controllers:** Handle incoming HTTP requests (`GET`, `POST`, `PUT`, `DELETE`) and return standard HTTP Status Codes (200 OK, 404 Not Found, etc.).
2.  **Services/Interfaces:** Contain the core business logic, injected via Dependency Injection (DI) to promote loose coupling.
3.  **Data Layer:** Manages all interactions with the Entity Framework `DbContext`.

## 💻 Setup & Installation
1. Clone the repository:
   ```bash
   git clone [https://github.com/suryanshkishor/OmniCart-Inventory-API.git](https://github.com/suryanshkishor/OmniCart-Inventory-API.git)
