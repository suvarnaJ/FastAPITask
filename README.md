# Super30 FastAPI GET API Task

## Project Objective

This project is a beginner-level FastAPI application created as part of the Super30 assignment.

The objective is to understand:

- FastAPI application creation
- FastAPI()
- @app.get()
- Static routes
- Dynamic routes
- URL path parameters
- Type hints
- JSON responses
- Running FastAPI using Uvicorn
- Swagger documentation
- ReDoc documentation

---

## Project Structure

super30-fastapi-get-api-task/

├── main.py
├── requirements.txt
└── README.md

---

## Installation

First, create a virtual environment.

### Windows

python -m venv venv

Activate the virtual environment:

venv\Scripts\activate

Install dependencies:

pip install -r requirements.txt

---

## Run the Application

Run the following command:

uvicorn main:app --reload

The application will run at:

http://127.0.0.1:8000

---

## Swagger Documentation

Open:

http://127.0.0.1:8000/docs

FastAPI automatically provides an interactive Swagger UI.

---

## ReDoc Documentation

Open:

http://127.0.0.1:8000/redoc

---

# Available APIs

## 1. Home

GET /

Example:

http://127.0.0.1:8000/

Response:

{
    "message": "Welcome to Super30 FastAPI"
}

---

## 2. Student

GET /student

Example:

http://127.0.0.1:8000/student

---

## 3. Course

GET /course

Example:

http://127.0.0.1:8000/course

---

## 4. Skills

GET /skills

Example:

http://127.0.0.1:8000/skills

---

## 5. Addition

GET /add/{num1}/{num2}

Example:

http://127.0.0.1:8000/add/10/20

Response:

{
    "result": 30
}

Another example:

http://127.0.0.1:8000/add/50/25

Response:

{
    "result": 75
}

---

## 6. Multiplication

GET /multiply/{num1}/{num2}

Example:

http://127.0.0.1:8000/multiply/5/8

Response:

{
    "result": 40
}

---

## 7. Square

GET /square/{number}

Example:

http://127.0.0.1:8000/square/9

Response:

{
    "number": 9,
    "square": 81
}

---

## 8. Even/Odd

GET /check/{number}

Example:

http://127.0.0.1:8000/check/17

Response:

{
    "number": 17,
    "type": "odd"
}

Another example:

http://127.0.0.1:8000/check/20

Response:

{
    "number": 20,
    "type": "even"
}

---

## 9. Age

GET /age/{age}

Example:

http://127.0.0.1:8000/age/25

Response:

{
    "age": 25,
    "message": "You are an adult."
}

---

## 10. Multiplication Table

GET /table/{number}

Example:

http://127.0.0.1:8000/table/7

Returns the multiplication table from 1 to 10.

---

## 11. Profile

GET /profile/{name}/{age}

Example:

http://127.0.0.1:8000/profile/Sudhanshu/37

Response:

{
    "name": "Sudhanshu",
    "age": 37
}

---

## 12. Number Analysis

GET /number/{number}

Example:

http://127.0.0.1:8000/number/25

Response:

{
    "number": 25,
    "square": 625,
    "cube": 15625,
    "even": false
}

---

## HTTP Methods

Only GET APIs are implemented in this assignment.

The following methods are NOT used:

- POST
- PUT
- PATCH
- DELETE

---

## Testing

The APIs can be tested using:

- Browser
- Swagger UI
- Postman
- Thunder Client
- curl

