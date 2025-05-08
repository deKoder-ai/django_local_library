# django_local_library
https://developer.mozilla.org/en-US/docs/Learn_web_development/Extensions/Server-side/Django

__Create Github Repo
Add a README file
Add .gitignore - python

__Clone Repo to Local Machine
git clone **SSH Link**

__Setup venv and Activate
cd **project directory**
python3 -m venv venv
source venv/bin/activate

__Install Django
pip install django

__Create Django Project
django-admin startproject **app name** .
(Note: The trailing . creates the project in the current directory)

__Create Requirements File
pip freeze > requirements.txt

__Create Django App
python3 manage.py startapp **next app name**

__Add **app name** to INSTALLED_APPS in config.settings.py
INSTALLED_APPS = [
    'django.contrib.admin',
    'django.contrib.auth',
    'django.contrib.contenttypes',
    'django.contrib.sessions',
    'django.contrib.messages',
    'django.contrib.staticfiles',
    '**app name**',
]

__Run Initial Migration
python3 manage.py migrate

__Create Superuser
python3 manage.py createsuperuser

__Commit to Github
git add .
git commit -m 'Skeleton Django Project'
git push origin main

__Run Dev Server
python3 manage.py runserver

http://localhost:8000/
http://localhost:8000/admin/