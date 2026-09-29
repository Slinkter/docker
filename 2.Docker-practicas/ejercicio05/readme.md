construir los 3 archivos
 - app.py
 - requirements.txt
 - DockerFile

construir la imagen

```bash 
docker build -t my-fastapi-app . 

docker run -p 8000:8000 my-fastapi-app 
docker run -d --name fastapi01 -p 8000:8000 my-app
```