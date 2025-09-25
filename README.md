# Insurance Policy Management System

A full-stack application built with ASP.NET Core 8 Web API and Angular 17.

## Tech Stack
- **Backend**: ASP.NET Core 8 Web API, Entity Framework Core, SQL Server
- **Frontend**: Angular 17 + Bootstrap 5
- **Database**: SQL Server (HARISHKAVANA/angular_project)

## Features
- JWT Authentication & Authorization
- Role-based access (Admin/User)
- Policy management (CRUD)
- Claims management
- File upload/download system
- Responsive Bootstrap UI

## Default Admin User
- **Email**: admin@insure.com
- **Password**: Admin@123
- **Role**: Admin

## Setup Instructions

### Backend Setup
1. Navigate to the backend directory:
   ```bash
   cd insu/insu
   ```

2. Restore NuGet packages:
   ```bash
   dotnet restore
   ```

3. Run the backend:
   ```bash
   dotnet run
   ```
   The API will be available at `http://localhost:5000`

### Frontend Setup
1. Navigate to the frontend directory:
   ```bash
   cd InsuranceApp
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   ng serve
   ```
   The app will be available at `http://localhost:4200`

## Database
The application uses Entity Framework Code First approach. The database will be automatically created when you first run the backend.

## API Endpoints
- `POST /api/auth/login` - User login
- `POST /api/auth/register` - User registration
- `GET /api/policies` - Get all policies
- `POST /api/policies` - Create policy (Admin only)
- `GET /api/claims` - Get claims (filtered by user role)
- `POST /api/claims` - Create claim
- `POST /api/uploads` - Upload file
- `GET /api/uploads/download/{id}` - Download file

## Project Structure
```
├── insu/insu/                 # Backend (ASP.NET Core)
│   ├── Controllers/           # API Controllers
│   ├── Models/               # Entity Models
│   ├── Data/                 # DbContext
│   └── uploads/              # File storage
└── InsuranceApp/             # Frontend (Angular)
    ├── src/app/
    │   ├── components/       # Angular Components
    │   ├── services/         # HTTP Services
    │   └── guards/           # Route Guards
```

## Usage
1. Start both backend and frontend servers
2. Navigate to `http://localhost:4200`
3. Register a new user or login with admin credentials
4. Explore the features based on your role (Admin/User)