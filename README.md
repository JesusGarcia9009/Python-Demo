# Python-Dajango-Demo
Demo de python con Django con REST FRAMEWORK

## Aplications
```
INSTALLED_APPS = [
    'django.contrib.admin',
    'django.contrib.auth',
    'django.contrib.contenttypes',
    'django.contrib.sessions',
    'django.contrib.messages',
    'django.contrib.staticfiles',
    # restframefork de django
    'rest_framework',
    # nueva aplicacion llamada tutoriales
    'tutorials.apps.TutorialsConfig',
    # CORS
    'corsheaders',
]
```

## DATABASE - postgres

```
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql',
        'NAME': 'django',
        'USER': 'postgres',
        'PASSWORD': 'postgres',
        'HOST': 'localhost',
        'PORT': '5432',
    }
}
```

## MIDDLEWARE - CORS
MIDDLEWARE = [
    'django.middleware.security.SecurityMiddleware',
    'django.contrib.sessions.middleware.SessionMiddleware',
    'django.middleware.common.CommonMiddleware',
    'django.middleware.csrf.CsrfViewMiddleware',
    'django.contrib.auth.middleware.AuthenticationMiddleware',
    'django.contrib.messages.middleware.MessageMiddleware',
    'django.middleware.clickjacking.XFrameOptionsMiddleware',
    # CORS
    'corsheaders.middleware.CorsMiddleware',
    'django.middleware.common.CommonMiddleware',
]

##### COMANDOS ######
## Comando para crear un proyecto Django
django-admin startproject name-app

## Comando para crear un modelulo dentro del proyecto django
- python manaje.py startapp name-modulo

## Inspeccionar base de datos
- python mysite/manage.py inspectdb

## Migraciones Iniciales de los proyectos o cuando hay cambios en la base de datos(aplica los cambios dentro del proyecto en la base de datos)
- python manage.py migrate
- python manage.py makemigrations
- python manage.py migrate

## Start server
- py manage.py runserver

## Creacion del super usuario
- py manage.py createsuperuser

## instalar driver para postgres
- pip install psycopg2


