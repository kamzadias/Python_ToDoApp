# Django ToDo app
Django ToDo app with authentication and with saving the list in the PostgreSQL.

## Installation

- Install libraries:

```shell
$ pip install django
$ pip install psycopg2 
```
- Install PostgreSQL

## Usage
- Create the database
- Go to NAMEOFPROJECT/settings.py:
 
```shell
- Change the DATABASES info

DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql',
        'NAME': 'DATABASE_NAME',
        'USER':'postgres',
        'PASSWORD':'',
        'HOST':'localhost'
    }
}
```
- Run a command in terminal
```shell
$ python manage.py migrate  
```
- Create a superuser
```shell
$ python manage.py createsuperuser 
```
- Run the server
```shell
$ python manage.py runserver  
```
## Examples
- Run the server and go to the link
```python
http://127.0.0.1:8000/
```
- Login by superuser account

After login or registration, you will see a simple interface where you can create, delete and search for your task.

![image](https://user-images.githubusercontent.com/68639981/150323078-1c0c3ff5-a349-46b9-a962-c622f766a593.png)
