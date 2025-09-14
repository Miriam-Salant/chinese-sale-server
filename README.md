# Chinese Sale – Server (Web API)

This repository contains the **ASP.NET Core Web API backend** for the Chinese Sale project.  
It manages authentication, business logic, and data persistence.

👉 Client (Angular) repository: [Chinese Sale – Client](https://github.com/Miriam-Salant/chinese-sale-client)

---

## 🚀 Features
- Authentication with JWT tokens
- Management user access secured with `[Authorize(Roles = "manager")]`
- Donors management:
  - View, add, update, delete donors
  - Search donors by name, email, or gift
- Gifts management:
  - View, add, update, delete gifts
  - Assign donors, categories, ticket price, optional image
  - Search by gift, donor, or number of buyers
- Purchases management:
  - View purchases, sort by most expensive / most purchased gifts
  - View buyer details
- Lottery:
  - Draw winners per gift
  - Generate reports (winners, total revenue)
---

## 🛠️ Technologies
- ASP.NET Core Web API (.NET 8)
- SQL Server
- Entity Framework Core
- JWT Authentication

---

## ⚙️ Setup & Run
```bash
git clone https://github.com/<your-username>/chinese-sale-server.git
cd chinese-sale-server
dotnet restore
dotnet ef database update   # create database from migrations
dotnet run

API will run on:
https://localhost:5001
http://localhost:5000
