# Project documentation for a Django Girls tutorial blog

## Introduction
The blog project was created using the Django framework, SQLite database, and deployed on pythonanywhere.com at https://marekdrag.pythonanywhere.com/. The aim of the project was to learn the basics of programming in Django and create a functional blog with the ability to add posts, comments, and edit/delete them by the administrator.

## Application Description
The project consists of two applications: blog and accounts. The blog application implements the functionality of adding posts and comments. Users can browse posts and add comments, but only logged-in users can add posts. The administrator can edit and delete posts and comments. The accounts application allows users to log in and register on the website.

## Cloning the repository

Clone the repository using the command below :
```bash
git clone https://github.com/UserMarekDrag/my-first-blog.git
```

Move into the directory where we have the project files : 
```bash
cd my-first-blog
```

Create a virtual environment :
```bash
# Create our virtual environment
python -m venv venv
```

Activate the virtual environment : <br><br>
windows
```bash
venv\scripts\activate
```
linux
```bash
source venv/bin/activate
```

Install the requirements :
```bash
pip install -r requirements.txt
```

Migrate Database
```bash
python manage.py migrate
```

Create Super User
```bash
python manage.py createsuperuser
```

### Running the App

To run the App, we use :
```bash
python manage.py runserver
```
> ⚠ Then, the development server will be started at http://127.0.0.1:8000/

## Deploying on pythonanywhere.com
To deploy the project on pythonanywhere.com, follow these steps:
Create an account on pythonanywhere.com and go to the Dashboard tab.
In the Files tab, create a new directory for project files.
Import the project from the Git repository: https://github.com/UserMarekDrag/my-first-blog.git
In the Web tab, create a new virtual application and configure its settings.
In the application settings, add paths to static files and media.
Update the database using the command: python manage.py migrate
Run the application server and check if the website works correctly.

## Summary
The blog project created using the Django framework and SQLite database was deployed on pythonanywhere.com. The project allows users to browse posts and add comments, and the administrator can edit and delete posts and comments. The project was a good tool for learning programming in Django and deploying on a web server.