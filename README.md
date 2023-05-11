### Notice
This code is from the great guide by Michael Herman as below.
https://testdriven.io/blog/dockerizing-flask-with-postgres-gunicorn-and-nginx/


### Build
```
$ docker-compose -f docker-compose.prod.yml up -d --build
$ docker-compose -f docker-compose.prod.yml exec web python manage.py create_db
```


### Down all images
```
$ docker-compose -f docker-compose.prod.yml down -v
```

### Debug
```
docker-compose -f docker-compose.prod.yml logs -f
```
