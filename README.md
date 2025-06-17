Created by Wan Nurqistina binti Rosmin

To-Do List Application
A simple, user-friendly To-Do List web application built with Django and styled with Bootstrap 5. The application allows users to create, view, update, and delete tasks, with a responsive interface suitable for both desktop and mobile devices.
Project Overview
This project is a basic task management system designed to demonstrate Django’s Model-View-Template (MVT) architecture. It uses SQLite for data storage and Bootstrap 5 for a modern, responsive frontend. The app is ideal for learning Django basics, including models, views, forms, templates, and URL routing.
Features

Create Tasks: Add tasks with a title, optional description, and completion status.
View Tasks: Display all tasks in a responsive card layout, with completed tasks visually distinguished.
Update Tasks: Edit task details or mark tasks as completed.
Delete Tasks: Remove tasks with a confirmation prompt.
Responsive UI: Built with Bootstrap 5 for a clean, mobile-friendly interface.
Admin Panel: Manage tasks via Django’s built-in admin interface.
Database: Uses SQLite for simplicity in development.

Prerequisites

Python 3.8 or higher
pip (Python package manager)
Virtual environment (recommended)
Git (optional, for cloning the repository)

How to Run Locally
Follow these steps to set up and run the application on your local machine:

Clone the Repository (if using Git):
git clone <repository-url>
cd todo_project


Create a Virtual Environment:
python -m venv venv


Activate the Virtual Environment:

On Windows:venv\Scripts\activate


On Mac/Linux:source venv/bin/activate




Install Dependencies:
pip install -r requirements.txt

The requirements.txt includes django and django-widget-tweaks.

Apply Database Migrations:
python manage.py migrate


Create a Superuser (optional, for admin access):
python manage.py createsuperuser


Run the Development Server:
python manage.py runserver


Access the Application:

Open your browser and visit http://127.0.0.1:8000/ to use the app.
Visit http://127.0.0.1:8000/admin/ to access the admin panel (log in with the superuser credentials).


Dependencies

django: Web framework for the backend.
django-widget-tweaks: For adding Bootstrap classes to Django forms.
bootstrap 5: Loaded via CDN for frontend styling.

Install dependencies using:
pip install django django-widget-tweaks

Usage

Home Page: View all tasks in a card layout, with options to edit or delete each task.
Add Task: Click “Add New Task” to create a task with a title, description, and completion status.
Edit Task: Click “Edit” on a task to update its details.
Delete Task: Click “Delete” and confirm to remove a task.
Admin Panel: Manage tasks (add, edit, delete) via /admin/.

Troubleshooting

Database Issues: If migrations fail, delete db.sqlite3 and the todo/migrations/ directory (except __init__.py), then rerun python manage.py makemigrations and python manage.py migrate.
Template Not Found: Ensure templates are in todo/templates/todo/ and APP_DIRS is set to True in settings.py.
Bootstrap Not Loading: Verify your internet connection for the Bootstrap CDN or host Bootstrap locally.
Form Styling Issues: Ensure django-widget-tweaks is installed and added to INSTALLED_APPS.

Future Enhancements

Add user authentication to restrict tasks to specific users.
Implement task categories or priority levels.
Add filtering to view completed or pending tasks.
Deploy the app to Heroku or another cloud platform.
Visualize task completion stats with a chart (e.g., using Chart.js).

Contributing
Contributions are welcome! Please fork the repository, create a new branch, and submit a pull request with your changes.
License
This project is licensed under the MIT License.
