# Z-Board Docker Deployment Notes

The basic-auth password in the .env file must **not** need to be escaped, e.g., only single `$` signs.
* ```cp .env.example .env```
* ```docker network create internal```
* ```docker network create proxy```
* ```docker-compose up --build```