docker-lamp-precise
=================

Building
--------
docker build -t bytekast/docker-lamp-precise .


Running
--------
docker run -d -p 2222:22 -p 80:80 -p 3306:3306 -e AUTHORIZED_KEYS="`cat ~/.ssh/id_rsa.pub`" bytekast/docker-lamp-precise


SSH
---
ssh -p 2222 root@${CONTAINER_IP}