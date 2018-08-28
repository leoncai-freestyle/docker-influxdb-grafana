# docker-influxdb-grafana
docker-compose up -d 

#Deploy for client server
docker-compose -f docker-compose-client.yml up -d
#Pass local env to docker
hostname=$HOSTNAME docker-compose -f docker-compose-client.yml up -d --build

