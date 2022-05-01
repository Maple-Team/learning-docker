## Redis
```sh
docker run -d -p 6379:6379 --name maple-redis --network maple-network --mount type=bind,source=$PWD/docker-data/redis/data,target=/bitnami/redis/data -e ALLOW_EMPTY_PASSWORD=yes --rm  bitnami/redis
```
## Mysql
```sh
docker run -p 3306:3306 -d -e ALLOW_EMPTY_PASSWORD=yes -e MYSQL_CHARACTER_SET=utf8mb4 -e MYSQL_COLLATE=utf8mb4_general_ci  --mount type=bind,source=$PWD/docker-data/mysql/data,target=/bitnami/mysql/data  -v $PWD/docker-data/mysql/my_custom.cnf:/opt/bitnami/mysql/conf/my_custom.cnf:ro  -e MYSQL_DATABASE=maple --name maple-mysql  --network maple-network bitnami/mysql:latest
```

## Mongodb

```sh
 docker run -d --name maple-mongodb -p 27017:27017 --network maple-network -e ALLOW_EMPTY_PASSWORD=yes -e MONGODB_EXTRA_FLAGS='--wiredTigerCacheSizeGB=2' --mount type=bind,source=$PWD/docker-data/mongodb/data,target=/bitnami/mongodb bitnami/mongodb
```
## php-mysql-nginx
https://github.com/Robert-Ro/sitepoint-docker-tutorial