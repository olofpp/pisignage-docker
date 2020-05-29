# pisignage-docker
Pisignage server for testing purpose. 


How to use.
1. git clone https://github.com/olofpp/pisignage-docker.git
2. cd pisignage-docker
3. docker-compose up -d

Note that media and license will be stored in a subfolder called storage.

docker-compose-traefik.yml is setup for my reverse proxy and can be started with following command. 
docker-compose -f docker-compose-traefik.yml up -d
