Some docker commands

docker run img_name (runs the image)

eg. docker run --name web01 -d -P 9080:80 nginx

docker images (shows available images)

docker ps (shows running containers)

docker ps -a (shows all containers)

docker inspect web01 (shows details)

docker build -t img_name . (builds the image from the docker file)

docker start container_name (starts the container)

docker stop container_name (stops container)

docker exec -it container_id bash (opens up terminal of the container)

docker rm container_id (removes container)

docker rmi image_id (removes image)

docker network ls (list network)

docker network inspect my_network (inspect network)

docker network create my_network (create network)

docker network connect my_network my_container (connect container to network)

docker network disconnect my_network my_container (disconnect container to network)

docker network rm my_network (remove network)

docker volume ls (list volumes)

docker volume inspect my_volume (inspect volume)

docker volume create my_volume (create a volume)

docker volume rm my_volume (remove volume)

docker volume prune (prune unused volume)

docker run -d -v my_volume:/app/data nginx or docker run -d --mount source=my_volume,target=/app/data nginx (mount a named volume)

docker run -d -v /app/data nginx or docker run -d --mount target=/app/data nginx (Mount an Anonymous Volume)

docker run -d -v /path/on/host:/app/data nginx or docker run -d --mount type=bind,source=/path/on/host,target=/app/data nginx (Mount a Host Directory as a Volume)

