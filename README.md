# docker_zabbix-server

Docker-compose para desplegar un servidor Zabbix.

---
#### Notas
usar la ip del contenedor "zabbix-agent" para la recolección de datos en zabbix-server

- docker inspect zabbix-agent | grep "IPAddress\":"
---

docker-compose stop

docker-compose rm -f

docker ps -aq

docker stop $(docker ps -aq)

docker rm $(docker ps -aq)
