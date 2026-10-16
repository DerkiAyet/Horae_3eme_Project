# Teacher Management System

A full-stack platform for managing teachers' schedules, absences and payments. An admin plans each teacher's timetable, records absences, and the app automatically calculates each teacher's payment based on their **grade**, **schedule** and **absences**.

> University group project (3rd year).

## Features

- Authentication with role-based access (admin / teacher)
- Schedule creation and management for each teacher
- Absence registration
- Automatic payment calculation according to grade, scheduled hours and absences
- Dedicated dashboard for each role
- REST API connecting the React frontend to the Django backend

## Roles

| Role | What they can do |
|---|---|
| **Admin** | Manage teachers, create schedules, register absences, calculate and review payments |
| **Teacher** | Log in to their own dashboard to see their schedule, absences and payment |

## Tech Stack

| Part | Technology |
|---|---|
| Frontend | React |
| Backend | Django (REST API) |
| Database | MySQL |

## Getting Started

### Prerequisites

- Python 3.9+
- Node.js 18+
- MySQL Server

### 1. Database

```sql
CREATE DATABASE teacher_management;
```

### 2. Backend

```bash
cd backend
python -m venv venv
venv\Scripts\activate          # Windows
# source venv/bin/activate     # macOS / Linux
pip install -r requirements.txt
```

Create a `.env` file (or edit your settings) with your database credentials, then run:

```bash
python manage.py migrate
python manage.py createsuperuser
python manage.py runserver
```

The API runs on `http://localhost:8000`.

### 3. Frontend

```bash
cd frontend
npm install
npm start
```
## My Role

**Ayet Halima Derki:** Frontend developer, API integration
