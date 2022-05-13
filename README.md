# Z-Board Docker Deployment Notes

The basic-auth password in the .env file must **not** need to be escaped, e.g., only single `$` signs.
* ```cp .env.example .env```
* ```docker network create internal```
* ```docker network create proxy```
* ```docker-compose up --build```


//Make sure that server uses the correct/same data for db connection as specified here in env

Dial into server
```docker exec -it api /bin/bash```

Execute
```php artisan migrate:fresh --seed```
