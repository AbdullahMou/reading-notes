# Docker

## Library Website and API

* Django REST Framework works alongside the Django web framework to create web APIs.
* We cannot build a web API with only Django Rest Framework; it always must be added to a project after Django itself has been installed and configured.

## First app

* The typical next step is to start adding apps, which represent discrete areas of functionality.
* A single Django project can support multiple apps.

## Models

* This is a basic Django model where we import models from Django on the top line and then create a class that extends it.
* We also include a `__str__` method so that

## Admin

* We can start entering data into our new model via the built-in Django app.
* But we must do two things first: create a superuser account and update `admin.py`

## Views
* The `views.py` file controls how the database model content is displayed. 
* Since we want to list all books we can use the built-in generic class ListView.

## URLs
* We need to set up both the project-level `urls.py` file and then one within the  `app`.
* When a user visits our site they will first interact with the `config/urls.py` file so let’s configure that first.
* Add the `include` import on the second line and then a new path for our  `app`.

## Webpage
* Now we can start up the local Django server and see our web page.

## Django REST Framework
* Django REST Framework is added just like any other third-party app.
* Make sure to quit the local server `Control + c` if it is still running. Then on the command line type the below.

## URLs
* Let’s start with our URL configs. Adding an API endpoint is just like configuring a traditional Django app’s routes. 

## Serializers

* **A serializer** translates data into a format that is easy to consume over the internet, typically JSON, and is displayed at an API endpoint.
* We will also cover serializers and JSON in more depth in following chapters.
* For now I want to demonstrate how easy it is to create a serializer with Django REST Framework to convert Django models to JSON.

## Browsable API
* With the local server still running in the first command line console, navigate to our API endpoint in the web browser at` http://127.0.0.1:8000/api/`
