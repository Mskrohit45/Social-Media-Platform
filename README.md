Social Media Project

This is a Django-based social media project that allows users to connect, share posts, and interact with each other.

Prerequisites

Before running the project, ensure you have the following installed:

Python (>=3.8)

Django (>=4.0)

Virtualenv (recommended for dependency management)

Installation & Setup

Clone the repository:

git clone https://github.com/yourusername/socialmedia.git
cd socialmedia

Create a virtual environment:

python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`

Install dependencies:

pip install -r requirements.txt

Apply database migrations:

python manage.py migrate

Create a superuser (for admin access):

python manage.py createsuperuser

Run the development server:

python manage.py runserver

Project Structure

manage.py - Entry point for Django administrative tasks.

socialmedia/ - Main project folder with settings and configurations.

apps/ - Contains different Django applications for modular development.

static/ - Holds static files like CSS, JavaScript, and images.

templates/ - HTML templates for frontend rendering.

Environment Variables

Create a .env file in the root directory and add the necessary configurations:

SECRET_KEY=your_secret_key
DEBUG=True
ALLOWED_HOSTS=*
DATABASE_URL=postgres://user:password@localhost:5432/db_name

Running Tests

To run tests, execute:

python manage.py test

Deployment

For production, ensure you:

Set DEBUG = False in settings.py.

Use a production-ready database like PostgreSQL.

Configure a WSGI server (e.g., Gunicorn, uWSGI).

Use a reverse proxy (e.g., Nginx, Apache).

License

This project is licensed under the MIT License.



