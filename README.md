<h1> Asynchronous Tasks with Django and Celery</h1>

<i> Setup </i>

```
python3 -m venv venv 
source venv/bin/activate
(venv) python3 -m pip install -r requirements.txt
```
<hr>
<h3>You'll also need to install Redis on your system: </h3>

<hr>
```
sudo install redis
```

<hr>

<h3> You need to start three processes that need to run at same time: </h3>

```
(venv) python3 manage.py migrate
(venv) python3 manage.py runserver
```

<h2> Redis server:</h2>

```
redis-server
```
<h2>Celery </h2>

```
(venv) python3 -m celery -A django_celery worker -l info
```


