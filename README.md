### Avito Devops Test

#### Prerequisites
Docker installed.
CORS extension on browser to test the app ( //TODO : fix the CORS problem )

#### Usage
docker-compose up

#### docker-compose file description



We have 4 services :
* Front:
Builds the dockerfile from the directory front and expose port 3000.
* Nginx :
Builds the dockerfile from the directory front and ties the container's port 3000 to the host's port 3000.
* Server :
Builds the dockerfile from the directory front and expose port 9999.
* API :
Builds the dockerfile from the directory api and expose port 8080.

All the services are linked together with docker compose.

Each Dockerfile is documented in the related directory
