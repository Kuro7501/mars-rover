docker build -t python-server .
docker run -d -p 8080:80 python-server

EXO 4
docker run --rm -v ${PWD}:/app -w /app -p 8080:80 python:3.11-slim python serveur.py

EXO 5
docker network create kuro-reseau

docker run -dit --name conteneur1 --network kuro-reseau alpine sh
docker run -dit --name conteneur2 --network kuro-reseau alpine sh

docker exec -it conteneur1 sh

ping conteneur2
