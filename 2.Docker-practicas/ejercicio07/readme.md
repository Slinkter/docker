docker volume create mysql-data

docker run -d --name my-sql-db -e MYSQL_ROOT_PASSWORD=mi-clave-secreta -v mylsql-data:/var/lib/mysql mysql:8.0

docker ps -a 

docker exec -it my-sql-db -u root -p 

-> activado mysql
-> CRUD  example.sql

docker ps
docker rm -f my-sql-db

-> crear otra base de datos

