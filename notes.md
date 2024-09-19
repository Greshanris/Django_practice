# Notes for Django Practice
I am practicing in Ubuntu 24.04.1, so shell scripting is mostly bash.

## Checking Python Version
```bash
python3 --version
```
## Creating Virtual Environment
```bash
python3 -m venv .venv
```
we can write any name instead of .venv

## Activating Virtual Environment
```bash
source .venv/bin/activate
```
if we wanted to deactivate, we can use
```bash
deactivate
```

## Installing Django on Virtual Environment
```bash
python3 -m pip install Django
```
To, check if the Django and Python is working as intended, we can use:
```bash
python3
```
enter, and python starts running:
```Python
import django
```
enter, and write
```Python
print(django.get_version())
```
This gave me output, 5.1.1

To Quit,
```Python
quit()
```
Now, we are outside python, but inside the virtual environment.

## Starting with Django
Now, inside the same virtual environment, to create a project with Django, we can use
```bash
django-admin startproject myproject
```
here, "myproject" is the projectname, and we can write anything here.

Now, we can see that there is "myproject" folder and inside the folder, there is another "myproject" folder and manage.py . It should be like this. 
Inside the "myproject" folder which is inside the main "myproject" folder there will be different py files such as init, asgi, settings, urls, and wsgi which we will be working on later.
