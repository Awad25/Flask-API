# Flask API Project

This project is a simple Flask-based RESTful API that uses SQLAlchemy for database management. It provides endpoints to manage users, including creating, retrieving, updating, and deleting user records.

## Features

- RESTful API built with Flask and Flask-RESTful
- SQLite database integration using Flask-SQLAlchemy
- User management with endpoints for CRUD operations
- Input validation using Flask-RESTful's `reqparse`
- Easy setup with a `requirements.txt` file for dependencies

## Project Structure

├── api.py # Main application file
├── create_db.py # Script to initialize the database
├── requirements.txt # Project dependencies
├── .env.example # Environment variables template
├── .gitignore # Git ignore file
├── instance/
│ └── database.db # SQLite database file (created after setup)
├── pycache/ # Compiled Python files
└── tests/ # Test files (if applicable)


## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Awad25/Flask-API.git
   cd Flask-API


   
2. Create and activate a virtual environment:
    ```bash
    python -m venv .venv
      
 On Windows:
  ```bash
  .venv\Scripts\activate
  ```
        
On macOS/Linux:
  ```bash
source .venv/bin/activate
```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
   
   extra step (Set up environment variables):
   ```bash
   cp .env.example .env
    ```
   
4. Initialize the database:
   ```bash
   python create_db.py
   ```

## Running the Application

Start the development server:
```bash
flask run
```
The API will be available at http://localhost:5000

## API Endpoints
User Management

GET /users: Retrieve all users

POST /users: Create a new user

GET /users/<id>: Get user by ID

PUT /users/<id>: Update user by ID

DELETE /users/<id>: Delete user by ID

## Notes

Make sure to recreate the database if the schema changes.
You can modify or extend the user model in api.py as needed.

