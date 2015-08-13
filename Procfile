web: gunicorn coffeed.wsgi --log-file -
web: python coffeed/manage.py collectstatic --noinput; bin/gunicorn_django --workers=4 --bind=0.0.0.0:$PORT coffeed/settings.py 
