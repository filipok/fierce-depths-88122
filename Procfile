web: waitress-serve --connection-limit 2000 --channel-timeout=300 --port=$PORT transverbis.wsgi:application
worker: python manage.py celery worker -c 1 --beat -l inf
