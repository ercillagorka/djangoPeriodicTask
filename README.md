djangoPeriodicTask
==================

Ejemplo de proyecto de django con periodic task

Instalar las dependencias:

```bash
$ pip install -r requirements.txt
```


Crear la base de datos:
```bash
$ python manage.py syncdb
```
Arrancar el servidor de redis y el worker de celery.

```bash
# El servidor de redis
$ redis-server
# En una nueva tab, el worker de celery
$ python manage.py celeryd worker -E
# Run Django
$ python manage.py runserver
```
