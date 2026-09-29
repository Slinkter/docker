# volumnes 

```bash

docker run -it --name mi-ubuntu-01 -v mis-datos:/app/data ubuntu

echo "este archivo es persistente" > archivo.txt


docker volume ls

docker rm mi-ubuntu-01


docker run -it --name mi-otro-ubuntu -v mis-datos:/app/data ubuntu

```