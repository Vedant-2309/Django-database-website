# Django-database-website (MacOS)

(It is assumed that the Django and Virtual environment are already set up)


### Here are the commands I ran

---

### 1. Creating the app

```
python3 manage.py startapp website
```

### 2. Add urls to website and add app to settings.py

```
from django.contrib import admin
from django.urls import path,include

urlpatterns = [
    path('admin/', admin.site.urls),
    path('', include('website.urls')),
]
```

Adding urls to our website on app level

```
INSTALLED_APPS = [
    'django.contrib.admin',
    'django.contrib.auth',
    'django.contrib.contenttypes',
    'django.contrib.sessions',
    'django.contrib.messages',
    'django.contrib.staticfiles',
    'website',
]
```

Adding our app to settings.py

