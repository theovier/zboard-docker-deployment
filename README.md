# Z-Board Docker Deployment

* ```cp .env.example .env```
* ```docker network create internal```
* ```docker network create proxy```
* ```docker-compose up --build```