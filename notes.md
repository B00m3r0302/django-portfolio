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
- 