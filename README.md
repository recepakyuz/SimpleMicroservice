# SimpleMicroservice

Ocelot  ApiGateway + Consul Service Discovery + .Net Core Web Api

docker stop $(docker ps -a -q)

docker rm $(docker ps -a -q)

docker network create mynet

docker run -d -p 8500:8500 --name consul --net mynet consul

docker run -d --net mynet testservice:latest

docker run -d --net mynet testservice:latest

docker run -d --net mynet testservice:latest

docker run -d -p 8080:80 --net mynet apigateway:latest

