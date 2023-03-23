# recipe-app-api
Recipe API Project 

### Run linting command :
```bash
docker-compose run --rm app sh -c "flake8"
```

### Run our Django project :
```bash
docker-compose run --rm app sh -c "django-admin startproject app ."
```
```bash
docker-compose run --rm app sh -c "python manage.py test"
```

### Run our core Django project :
```bash
docker-compose run --rm app sh -c "python manage.py startapp core"
```

### Check the availibility of the database :
```bash
docker-compose run --rm app sh -c "python manage.py wait_for_db"
```
### Check the test and linting :
```bash
docker-compose run --rm app sh -c "python manage.py test && flake8"
```