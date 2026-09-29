debe ubicarse en la carpeta para ejecutar
/home/user/docker/ejercicio03

```bash
docker build -t mi-script-python . 
```

```bash
user@msi:~/docker/ejercicio03$ docker build -t mi-script-python .
```

```bash
user@msi:~/docker/ejercicio03$ docker images
IMAGE                     ID             DISK USAGE   CONTENT SIZE   EXTRA
mi-script-python:latest   34cd70294c8f        183MB           45MB
```

```bash
docker run --rm mi-script-python
```