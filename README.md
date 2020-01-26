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

| METHOD        | URL           | REQUEST  |DESCRIPTION|
| ------------- |-----------------------------------:|:--------:|:----------:|
| GET      |http://localhost:8000/api/employee/||Get all employees|
| GET      |http://localhost:8000/api/employee/{id}||Get one employee by id|
| POST     |http://localhost:8000/api/employee/    |       |Create employee|