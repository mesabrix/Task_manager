Task Manager - Django CRUD Application

This Task Manager is a web-based application built with Django, enabling users to manage tasks efficiently with CRUD (Create, Read, Update, Delete) functionality.

Prerequisites

Before setting up the project, ensure you have the following installed:

Python (version 3.8 or later)

pipenv (Python package manager)

Virtual environment

Django (install using pip install django)

PyMySQL (install using pip install pymysql)

Project Setup

Clone the Repository

git clone https://github.com/your-username/task-manager.git
cd task-manager

Set Up a Virtual Environment

For Windows:

python -m venv venv
venv\Scripts\activate

For macOS/Linux:

python3 -m venv venv
source venv/bin/activate

Install Required Packages

pip install -r requirements.txt

Configure the Database

Ensure MySQL is installed and running. Then, modify settings.py to configure the database connection:

DATABASES = {
'default': {
'ENGINE': 'django.db.backends.mysql',
'NAME': "task_manager",
'HOST': '127.0.0.1',
'USER': 'root',
'PASSWORD': '',
'PORT': '3306',
}
}

Run Migrations

python manage.py makemigrations
python manage.py migrate

Launching the Application

Start the Django development server with:

python manage.py runserver

By default, the application will be available at:

http://127.0.0.1:8000/

Features

Add new tasks

View task details

Edit existing tasks

Remove tasks

Admin dashboard for task administration

