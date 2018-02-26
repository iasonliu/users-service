## FLASK-USERSERVICE [![Build Status](https://travis-ci.org/iasonliu/users-service.svg?branch=master)](https://travis-ci.org/iasonliu/users-service)

### Common Commands

Build the images:
```
$ docker-compose -f docker-compose-dev.yml build
```
Run the containers:
```
$ docker-compose -f docker-compose-dev.yml up -d
```
Create the database:
```
$ docker-compose -f docker-compose-dev.yml \
  run users-service python manage.py recreate_db
```

Seed the database:
```
$ docker-compose -f docker-compose-dev.yml \
  run users-service python manage.py seed_db
```
Run the tests:
```
$ docker-compose -f docker-compose-dev.yml \
  run users-service python manage.py test
```

Run the tests with coverage:
```
$ docker-compose -f docker-compose-dev.yml \
  run users-service python manage.py cov
```

Run checking stylistic and programming errors:
```

```
