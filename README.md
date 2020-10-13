# Docker Commands
* docker inspect -f '{{.NetworkSettings.IPAddress}}' <containerid>
  - -f --> Format string
 ``` docker stat```
- docker container ps
~- docker container ls
- docker contaier run -it --network <mynetwork> --name <name> nginx bash
- docker container ls -a
^ docker container exec -it containername <commands>
`- docker container port <containerid>
docker network ls
docker network -f drive=bridge
docker network ls --format '{{.ID}}: {{.Driver}}'
docker network inspect <networkid>
docker network create mynetwork
docker network connect mynetwork containerid
docker volume ls
docker volume inspect <volume name>
docker run -d --mount source=myvol,destination=/var/lib/mysql <imagename>
docker run -d --mount type=bind source=$(pwd),target=/app <imagename>
