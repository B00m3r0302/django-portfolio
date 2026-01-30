# Commands to start the Django project
```bash
uv init
```
```bash 
uv venv
```
```bash
rm main.py
```
```bash
uv add django
```
```bash
uv run django-admin startproject portfolio .
```
- Start dev server with
```bash
uv run manage.py runserver
```
- Create app with
```bash
uv run manage.py startapp <appname>
```
- Register your app by adding it to installed apps in settings.py under `portfolio`
- Register url path in urls.py
- Migrations set up the database that we are working with.
- Make migrations with 
```bash
uv run manage.py makemigrations
```

- To apply changes to DB from a model change run:
```bash
uv run manage.py makemigrations
```

```bash
uv run manage.py migrate
```

- Django shell can help you put stuff in the database with
```bash
uv run manage.py shell
```

- Use Django ORM to add stuff to database

```Django
from projects.models import Project
```

```Django
p1 = Project(title="Test Project", description="This is a test", technology="Django", image="testproject.png")
```

```Django
p1.save()
```

- Retrieve objects with

```Django
results = Project.objects.all()
```

```Django
results
```

- Specific

```Django
p = results[0]
```

```Django
# Return title or field
p.title
```

- Logic syntax
{%logic%}

- variables
{{variable}}

### Creating a superuser
```bash
uv run manage.py createsuperuser
```

#### Register models
in admin.py




