# REST API CRUD

## Local deployment

### Run app
- Execute commands in the terminal
    - Enter the project folder: `cd <folder_name>`
    - Create virtual environment: `virtualenv .venv`
    - Activate virtual environment: `source .venv/bin/activate`
    - Install project dependencies: `pip install -r requirements.txt`
    - Up database: `docker-compose up -d`
    - Run migrations `python manage.py migrate`
    - Run server `python manage.py runserver`

### Endpoints

*URL BASE*

Development: [http://localhost:8000/](http://localhost:8000/)

Production:  [https://rest-api-basic.herokuapp.com/](https://rest-api-basic.herokuapp.com/)

| METHOD   | URL               | DESCRIPTION            |
| ---------|:-----------------:|:----------------------:|
| GET      | api/employee/     | Get all employees      |
| GET      | api/employee/{id} | Get an employee by id  |
| POST     | api/employee/     | Create employee        |
| PUT      | api/employee/{id} | Update an employee     |  
| PATCH    | api/employee/{id} | Update an employee     |  
| DELETE   | api/employee/{id} | Delete an employee     |  

REQUEST

```
{ 
    "fullname": "string",
    "document_number": "string",
    "mobile_number": "string"
} 
```
