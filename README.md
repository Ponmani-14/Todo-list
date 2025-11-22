Django MySQL Todo App 📝

A simple Todo app built with Django and MySQL demonstrating basic CRUD operations (Create, Read, Update, Delete) with a single-page interface.

Features

Add, edit, delete todos

Uses MySQL for persistent storage

Simple front-end using Django Templates

Tech Stack

Django | MySQL | PyMySQL | VS Code | HTML/CSS

Setup
git clone https://github.com/<your-username>/django-mysql-todo.git
cd django-mysql-todo
python -m venv venv
# Windows PowerShell
.\venv\Scripts\Activate.ps1
pip install -r requirements.txt


MySQL setup

CREATE DATABASE taskmanager CHARACTER SET utf8mb4 COLLATE utf8mb4_general_ci;
CREATE USER 'root'@'localhost' IDENTIFIED BY 'yourpassword';
GRANT ALL PRIVILEGES ON taskmanager.* TO 'root'@'localhost';
FLUSH PRIVILEGES;


Update mysite/settings.py with your DB credentials, then run:

python manage.py makemigrations
python manage.py migrate
python manage.py runserver


Visit http://127.0.0.1:8000
 to use the app.
