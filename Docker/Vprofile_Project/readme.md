Create and organization name vprocontainers and 3 repository for web, db and app in dockerhub within that organization.
Name them respectively vprofileweb, vprofiledb and vprofileapp.

write your script in the docker-compose.yml file.
cd into the vprofile project and run docker compose build from the terminal.
To start the containers after they are built, run docker compose up -d
docker compose ps (list containers)
docker compose logs (show logs)
docker compose down (stop and remove container)
docker system prune -a (remove all stopped containers, networks, images, caches)

docker login (login into docker and provide your username and password in the terminal)
docker push vprocontainers/vprofileweb (push images in dockerhub account)
docker push vprocontainers/vprofiledb
docker push vprocontainers/vprofileapp
