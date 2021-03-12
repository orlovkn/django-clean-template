Django Clean Template
===
This is a clean Django template that gives you an opportunity to start your Django project as fast as it is possible.

All you need to do is clone this repo, run docker-compose file, and that's it.

* as a database, we are using **PostgreSQL**.
* also, this project includes a **flake8** config file.
* as a CI system, we added a config file for [Travis CI](https://travis-ci.com/). 

## The main command are:

### build project and run server
```
docker-compose up
```

### create a new app
```
docker-compose run --rm app sh -c "python manage.py startapp user"
```

### make migrations
```
docker-compose run --rm app sh -c "python manage.py makemigrations core"
```

### run tests with flake8
```
docker-compose run --rm app sh -c "python manage.py test && flake8"
```