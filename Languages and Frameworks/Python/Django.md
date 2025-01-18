
## Getting Started

#### Installation
- `pip install Django`

#### Creating Project
1. Creating your first project
	1. `django-admin startproject mysite`
	2. `startproject` is used to first create the project
2. To run:
	1. `python manage.py runserver <port_nr>`


#### File Structure

```
mysite/
	manage.py
    mysite/
        __init__.py
        settings.py
        urls.py
        asgi.py
        wsgi.py
```

###### Levels:
1. `manage.py` level -- a.k.a. Root Level
2. Project Level (inside the project directory)
3. App level

<img src="https://www.interviewbit.com/blog/wp-content/uploads/2022/06/Model-768x263.png">


###### Root Level
- `manage.py`:
	- Sets env variable and configs
	- Django’s command-line utility for administrative tasks.
	- points to your project’s settings.py file.
	- Command options:
		```
		$ django-admin <command> [options]
		$ manage.py <command> [options]
		$ python -m django <command> [options]
		```

###### Project Level:
- settings.py:
	- Defines configuration, base_dir, secret keys, debug options, allowed_hosts, **installed_apps**, **middleware**, root_url, templates, databases, auth_password_validations, timezone, Language, static_url, default_auto_field
- urls.py
	- Routing url file.
- asgi.py
- wsgi.py
- views.py:
	- Controller: Functionality/business logic
- model.py
	- Database models



#### Jinja2 Templates

- Django template language (DTL) --> Internal Template for Django
- Popular Alternative: Jinja2
- 