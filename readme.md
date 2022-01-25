# Django


# 0. Installation

- First install Django from the official website. 

*How do you start a project?*
```shell
# Initiate a new project
django-admin startproject mysite
```


# 1. File Structure

*What are the file structure and what do they mean?*

*Structure:*

mysite/
    manage.py
    mysite/
        __init__.py
        settings.py
        urls.py
        asgi.py
        wsgi.py

*What are they for?*

*Meanings:*
- The outer mysite/: root directory is a container for your project. 
- manage.py: A command-line utility that lets you interact with this Django project in various ways. 
    - url: https://docs.djangoproject.com/en/4.0/ref/django-admin/
- The inner mysite/ directory is the actual Python package for your project. Its name is the Python package name you’ll need to use to import anything inside it (e.g. mysite.urls).
- mysite/__init__.py: An empty file that tells Python that this directory should be considered a Python package.
url: https://docs.python.org/3/tutorial/modules.html#tut-packages
- mysite/settings.py: Settings/configuration for this Django project. Django settings will tell you all about how settings work.
- mysite/urls.py: The URL declarations for this Django project; a “table of contents” of your Django-powered site. You can read more about URLs in URL dispatcher.
- mysite/asgi.py: An entry-point for ASGI-compatible web servers to serve your project. See How to deploy with ASGI for more details.
- mysite/wsgi.py: An entry-point for WSGI-compatible web servers to serve your project. See How to deploy with WSGI for more details.

*How do you start a server?*

```py
python manage.py runserver
```

*WARNING: Now’s a good time to note: don’t use this server in anything resembling a production environment. It’s intended only for use while developing. (We’re in the business of making*

# 2. Start an App

*how do you start an app?*

```shell
python manage.py startapp polls
```

Structure
```
polls/
    __init__.py
    admin.py
    apps.py
    migrations/
        __init__.py
    models.py
    tests.py
    views.py
```

# 3. Create a view
