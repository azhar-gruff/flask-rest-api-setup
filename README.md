# Flask Rest API Setup

Initial scaffolding for a flask rest API development. Starter template for building your Flask and Flask Rest API applications.

## Features
- Gunicorn server setup
- Database migration setup for SQLAlchemy Models
- JWT authentication at `<your-host>/api/v1/login`
- Url to register your admin and users at `<your-host>/api/v1/signup`
- Provisioned route file for all your routes with admin blueprints
- Test environment setup

## Built With

This App was developed with the following stack:

- Python
- Flask
- Flask-restful
- Postgres DB
- Gunicorn Web Server

## Requirements
- Python 3.6+
- Python pip
- Postgres SQL

## Installation
- fork this repository
- create a .env file as shown in the env_example file
- setup your database 
- on the terminal cd into the app folder 
- run `pip install -r requirements.txt` to install required modules
- run `python manage.py db init ` to setup alembic migrations
- run `python manage.py db migrate -m='<your migration message>'` to create migration files
- then run `python manage.py db upgrade` to create tables

## Running the App
- on the terminal run `gunicorn main:app`
- To run app on a specific port use `gunicorn -127.0.0.1:port main:app`

## Usage
- `src/api/resources` --- flask-restful resources for your project
- `src/models` --- SQLAlchemy models and schema
- `src/routes/api` --- contains all your route definition
- `src/utils` --- contains validations, security and helper files
- `src/middlewares` --- define your middleware files here
- You can modify the app to suit your need.
- Happy usage.

## Credits
solnsumei@gmail.com
