docker run -it --name mi-ubuntu ubuntu:20.04 bash
apt-get update
apt-get install nano -y
echo 'hola docker' > hola.text
cat hola.text
exit
docker ps -a
docker rm mi-ubuntu
