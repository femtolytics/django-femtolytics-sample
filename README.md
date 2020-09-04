# django-femtolytics-sample

This is a sample Django project showing how to integrate [django-femtolytics](https://github.com/femtolytics/django-femtolytics) into your own Django project or to use as a starting point to deploy your own instance of django-femtolytics.

You can find a hosted version of django-femtolytics at [femtolytics.com](https://femtolytics.com)

## Getting Started

Here is a quick step-by-step on how to clone, and get this Django project running.

```
git clone https://github.com/femtolytics/django-femtolytics-sample
cd django-femtolytics-sample
pip -r requirements.txt
./manage.py migrate
./manage.py createsuperuser
./manage.py runserver 
```

A few notes: 
- You will probably want to create a virtual environment before executing the pip command. 
- Make sure to change the DJANGO_SECRET and DEBUG flags before deploying this to production.
- The API endpoint is setup to be `analytics/api/v1`, so make sure to configure your Femtolytics client to point there.