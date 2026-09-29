crear los 3 archivos
 - app.py
 - Dockerfile
 - requirements.txt

construir imagen 
```bash
liam@DESKTOP-UV2PAAQ:~/github/docker/2.Docker-practicas/ejercicio04$ docker build -t flask-app .

```

ejecutar imagen
```bash
docker run -p 5000:5000 flask-app 
```

ejecutar imagen en segundo plano
```bash
docker run -d -p 5000:5000 flask-app
```




reconstruire imagen 
docker build --no-cache -t flask-app .
