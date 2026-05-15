# SmartAttendance System

A web-based student attendance management system built with Flask and PostgreSQL.

## Features
- **Student Management:** Register new students with roll number, name, email, and phone contact.
- **Attendance Tracking:**
  - Automated check-in/check-out recording.
  - Daily status tracking.
  - Prevents duplicate check-ins or missing check-out errors.

## Screenshots

### Main Attendance Interface
![Attendance Interface](image/Attendance.png)

### Add Student Interface
![Add Student](image/Add%20Student.png)

## Prerequisites
- Python 3.x
- PostgreSQL Database

## Setup Instructions

1. **Clone the repository:**
   ```bash
   git clone <your-repo-url>
   cd SmartAttendance
   ```

2. **Install Dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Database Configuration:**
   Ensure your PostgreSQL instance is running. Update the `DB_CONFIG` dictionary in `app.py` with your database credentials:
   ```python
   DB_CONFIG = {
       "host": "localhost",
       "database": "attendance_db",
       "user": "your_username",
       "password": "your_password",
       "port": "5432"
   }
   ```

4. **Initialize Database:**
   Run the SQL commands provided in `schema.sql` within your PostgreSQL database to create the necessary tables.

5. **Run the Application:**
   ```bash
   python app.py
   ```
   The application will be accessible at `http://127.0.0.1:5000`.

## Built With
- [Flask](https://flask.palletsprojects.com/) - Web Framework
- [PostgreSQL](https://www.postgresql.org/) - Database
- [Psycopg2](https://www.psycopg.org/) - PostgreSQL adapter for Python
