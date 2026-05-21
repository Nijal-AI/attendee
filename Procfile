web: gunicorn attendee.wsgi --bind 0.0.0.0:8080 --workers 2 --timeout 120
worker: celery -A attendee worker -l info
scheduler: python manage.py run_scheduler
