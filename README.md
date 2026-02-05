# CMS Project

A Content Management System built with Spring Boot (Backend) and React/Vite (Frontend).

## Prerequisites
- Java 17 or higher
- Node.js 18 or higher
- MySQL Database

## Getting Started

### 1. Database Setup
Ensure you have a MySQL database running. The application is configured to create the database `cms` if it doesn't exist.
- **URL**: `jdbc:mysql://localhost:3306/cms`
- **Username**: `root`
- **Password**: `root@1234`
*(Update `src/main/resources/application-dev.yml` if your credentials differ)*

### 2. Backend (Spring Boot)
Open a terminal in the root directory (`cms`) and run:

```bash
# Linux/Mac
./mvnw spring-boot:run -Dspring-boot.run.profiles=dev

# Windows
.\mvnw spring-boot:run "-Dspring-boot.run.profiles=dev"
```
The backend will start on **http://localhost:8080**.

### 3. Frontend (React + Vite)
Open a new terminal in the `cms-admin` directory:

```bash
cd cms-admin
npm install
npm run dev
```
The frontend will start on **http://localhost:3000**.

## Login Credentials
A default admin user is created automatically on startup:
- **Email**: `admin@example.com`
- **Password**: `admin123`

## Troubleshooting
- **500 Error / Login Issues**: If you face login issues, restart the backend. The system automatically resets the admin password to `admin123` on startup.
