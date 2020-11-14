# django-docker-template

1. Create your django app

docker-compose run web django-admin your_super_awesome_project . 

2. Test your app bootstrapping

In your_super_awesome_project/settings.py

Look 
ALLOWED_HOSTS = []

And change it for
ALLOWED_HOSTS = ["*"]

docker-compose run web python manage.py runserver 0.0.0.0:8080

3. Generate apps

docker-compose run web python manage.py startapp blazingapp
