# Django Todo App Readme
This Django-based Todo App is a simple web application that allows users to manage their tasks. Users can register, log in, create, update, delete, and mark tasks as complete. This readme file will guide you through setting up and running the application.

# Prerequisites
Before you get started, make sure you have the following software installed on your system:

Python (3.10 or higher)
Django (4.2 or higher)
Pipenv (optional but recommended for managing virtual environments)
Installation
Clone the repository to your local machine:

bash
Copy code
git clone https://github.com/utso1707097/django-todo-app.git
cd django-todo-app
Create a virtual environment (optional but recommended):

bash
Copy code
pipenv install
pipenv shell
Install the project dependencies:

bash
Copy code
pip install -r requirements.txt
Create a database and apply migrations:

bash
Copy code
python manage.py migrate
Configuration
Create a .env file in the project's root directory and configure the following environment variables:

env
Copy code
DEBUG=True
SECRET_KEY=your_secret_key
EMAIL_HOST=your_email_host
EMAIL_PORT=your_email_port
EMAIL_HOST_USER=your_email@example.com
EMAIL_HOST_PASSWORD=your_email_password
Replace the placeholders with your actual values. Make sure to set DEBUG to False in a production environment.

Update the ALLOWED_HOSTS list in settings.py to specify which domains are allowed to access the application.

Configure your database settings in settings.py if you are not using the default SQLite database.

Usage
Create a superuser to access the Django admin panel (optional but recommended):

bash
Copy code
python manage.py createsuperuser
Start the development server:

bash
Copy code
python manage.py runserver
Access the application in your web browser at http://localhost:8000.

Register a new user account or use the superuser account to log in.

Use the app to create, update, delete, and mark tasks as complete.

# Features
User Authentication: Users can register, log in, and log out and search for todos.
Task Management: Users can create, read, update, and delete tasks.
Complete Status: Users can mark tasks as complete or incomplete.
User-specific Data: Each user has their own set of tasks.
Django Admin Panel: Access the admin panel at http://localhost:8000/admin to manage users and tasks easily.
Contributing
Contributions to this project are welcome! If you find a bug or have suggestions for improvements, please open an issue or submit a pull request.

License
This project is licensed under the MIT License - see the LICENSE file for details.

Acknowledgments
This project was created using the Django web framework.
Special thanks to the Django community for their excellent documentation and support.
Enjoy using the Django Todo App! If you have any questions or need further assistance, please don't hesitate to reach out.
