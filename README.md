### Avito Devops Test

#### Prerequisites
Docker installed.

#### Usage
docker-compose up

#### docker-compose file description

We define a network for our apps, using the 'bridge' network driver.

We have 3 services :
	- front:
	Builds the dockerfile from the directory front and expose port 3000.
	- nginx :
	Builds the dockerfile from the directory front and ties the container's port 3000 to the host's port 3000.
	- server :
	Builds the dockerfile from the directory front and expose port 9999.
	- API :
	Builds the dockerfile from the directory api and expose port 8080.