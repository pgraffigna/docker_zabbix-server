# docker_zabbix-server

Docker-compose para desplegar un servidor Zabbix.

---
#### Notas
docker inspect zabbix-agent | grep "IPAddress\":"
- usar la ip del contenedor "zabbix-agent" para la recolección de datos en zabbix-server

docker-compose stop
docker-compose rm -f

docker ps -aq
docker stop $(docker ps -aq)
docker rm $(docker ps -aq)