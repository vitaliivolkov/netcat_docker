# netcat_docker
docker network create test
docker build -t ncserver .
docker build -t ncsclient .
docker container run --network test_network -p 1234:1234 ncserver
docker container run --network test_network --link=ncserver ncserver
