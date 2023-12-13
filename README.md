# djangoDemo
django demo

## Info

```
Python 3.9.0
django 4.2.7
```


## Install

```
$ python -m pip install Django
```

## Start

Creating a project
```
$ django-admin startproject myWeb

myWeb/
    manage.py
    myWeb/
        __init__.py
        settings.py
        urls.py
        asgi.py
        wsgi.py
```

啟動
```
$ cd myWeb
$ python manage.py runserver

#更換 port
python manage.py runserver 0.0.0.0:8000
```

建立新項目
```
$ python manage.py startapp polls

polls/
    __init__.py
    admin.py
    apps.py
    migrations/
        __init__.py
    models.py
    tests.py
    views.py
```

TIME_ZONE
```
# settings.py
TIME_ZONE = 'Asia/Taipei'
```

資料庫配置
```
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.sqlite3',
        'NAME': BASE_DIR / 'db.sqlite3',
    }
}

$ python manage.py migrate
