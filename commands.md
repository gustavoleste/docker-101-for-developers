# Commands:

> `docker run -d -p 80:80 docker/getting-started`

> `docker build -t getting-started .`

> `docker run -dp 3000:3000 getting-started`

> `docker ps`

> `docker stop <the-container-id>`

> `docker rm <the-container-id>`

> `docker rm -f <the-container-id>`

> `docker tag getting-started YOUR-USER-NAME/getting-started`

> `docker push YOUR-USER-NAME/getting-started`

>`docker volume create todo-db`

>`docker run -dp 3000:3000 -v todo-db:/etc/todos getting-started`

>`docker volume inspect todo-db`

>` docker run -dp 3000:3000 -w /app -v "$(pwd):/app" node:12-alpine sh -c "yarn install && yarn run dev"`

>`docker network create todo-app`

>`docker run -d --network todo-app --network-alias mysql -v todo-mysql-data:/var/lib/mysql -e MYSQL_ROOT_PASSWORD=secret -e MYSQL_DATABASE=todos mysql:5.7`

>`docker exec -it <mysql-container-id> mysql -p`

>`docker-compose up -d`