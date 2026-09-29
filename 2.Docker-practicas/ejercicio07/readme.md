```bash
docker volume create mysql-data
```

```bash
docker run -d --name container-mysql -e MYSQL_ROOT_PASSWORD=secreto123 -v mylsql-data:/var/lib/mysql mysql:8.0
```

```bash
docker inspect container-mysql  | grep MYSQL
                "MYSQL_ROOT_PASSWORD=secreto123",
                "MYSQL_MAJOR=8.0",
                "MYSQL_VERSION=8.0.46-1.el9",
                "MYSQL_SHELL_VERSION=8.0.46-1.el9"
```

```bash
docker ps -a 
```

```bash
docker exec -it container-mysql mysql -u root -p

secreto123
```

-> activado mysql CRUD  
-> example.sql 

```bash
docker ps
docker rm -f container-mysql
```

-> crear otra base de datos , usar el volumen

```bash
docker volume ls
```
```bash
docker run -d --name mi-sql-db-nuevo -e MYSQL_ROOT_PASSWORD=secreto123 -v mysql-data:/var/lib/mysql mysql:8.0

docker exec -it mi-mysql-db-nuevo mysql -u root -p

```