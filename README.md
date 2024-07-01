# sunkenland

OLD:
Files to create the Sunkenland dedicated server on Ubuntu using Docker and Wine.

You can find the Docker image on Docker Hub:
https://hub.docker.com/r/adrianhowchin/sunkenland

To run the server, please see the instructions in the Docker Hub link above.

To see which versions this works against, see the Docker link above.


NEW:
clone repo
CD to directory
docker build -t sunkenland-mod .
docker run -d -p 27015:27015 --name suckenland_mod --cpus="2" --memory=8g -e "dPASSWORD=MYPASSWORD" -e "dGUID=MYGUID" -e "dREGION=MYREGION" --volume /opt/sunkenland/Worlds:/opt/sunkenland/Worlds sunkenland-mod
