# BudgetApp-System-Design
# SmartBudget: Full-Stack Enterprise Architecture

This project is a multi-repo personal finance engine designed to bridge the gap between complex banking data and user-friendly visualizations. 

## 🏗 System Topology

The system is split into two specialized repositories to ensure scalability and clean separation of concerns:

### 1. [Private] BudgetingApp (Backend)
* **Core:** .NET 8 Web API
* **Data Layer:** Entity Framework Core with SQL Server
* **Patterns:** Repository Pattern, Dependency Injection, and custom LINQ extensions for financial data flattening.
* **Security:** JWT Authentication and Role-Based Access Control.

### 2. [Private] BudgetingAppUI (Frontend)
* **Core:** Angular 18 & TypeScript
* **State Management:** RxJS for real-time balance updates.
* **Styling:** Tailwind CSS for a responsive, mobile-first design.
* **Deployment:** Hosted via Azure Static Web Apps with integrated CI/CD pipelines.

## 🔄 Integration Logic
The UI communicates with the API via a RESTful interface. I utilized **Docker** to containerize the local development environment, ensuring the SQL database, API, and Angular frontend work in sync regardless of the host machine.

## 📅 Project Status & Roadmap
- [x] Core API Architecture (.NET 8)
- [x] Database Schema Design (SQL Server)
- [ ] Currently Working: Angular 18 Signal implementation for real-time balance updates.
- [ ] Future: Azure DevOps CI/CD Pipeline setup.
