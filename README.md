# docker_zabbix-server

Docker-compose para desplegar un servidor Zabbix.

---
#### Notas

- contraseña por defaut Admin : zabbix

-  Agregar hosts:
  - Configurations --> Hosts
  - En Agent Interfaces: 
     - Usar la ip del contenedor "zabbix-agent" para monitorear al Servidor Zabbix 
     - docker inspect zabbix-agent | grep "IPAddress\":" 

- Al agregar hosts tener en cuenta los templates