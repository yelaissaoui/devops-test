### Description
This project is a Golang API accepting in the query string a number as parameter, and calculate the factorial of this number by sending a request to the Factorial TCP server.

### Docker File description

To build and run the application,we a are using a Dockerfile.
Based on golang:1.8 image from dockerhub, we copy the work directory into the container, then we install the prerequisites before starting the app.


### Usage
Use the docker compose file from the project root directory.

---- ONLY FOR TEST PURPOSE ----
You can build and run the Golang API in a standalone mode using :
`docker build -t devops-test_api .`
`docker run --name API -dt devops-test_api`

### TODO
* Register the API IP:port in a service discovery once UP
* We are doing a dirty trick to clean some data in Line 69, Can you explain why we need it ?
