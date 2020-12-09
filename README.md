# django-made-easy

# Step-01: Create a Django Project
## Creating project: django-admin startproject <name of the project>
  
  ### __init__.py
  ### manage.py
  ### settings.py
  ### urls.py
  ### wsgi.py
  ### project_name
  
## Creating Django App: python manage.py startapp <name of the app>
  ### HelloApp:
  #### migrations
  #### __init__.py
  #### admin.py
  #### apps.py
  #### models.py
  #### tests.py
  #### views.py
  
## Creating Virtual Environment: python3 -m  venv myEnv

## Activating vEnv: source myEnv/bin/activate

## Deactivating myEnv: deactivate

## Installing Django: pip install django

## Show files & folders: ls

## Pulling: git pull

# Go to views.py: 

## Importing HttpsResponsefrom django.http import HttpResponse

## Create views:
### def index(request):
      ### return HttpResponse("My Portfolio)

## Create url.py file in the app level:
### Import 'path' & 'views inside urls.py: 
#### from django.urls import path
#### from . import views
#### urlpatterns = [
###  path("", views.index)
### ]


## Got to project level urls.py and include the app inside 'urlpatterns' and import 'include' function
### path("", include("portfolio_app.urls")),
