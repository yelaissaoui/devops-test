### Description
This project is a simple TCP server written in C, it accepts a connection, expect a number as an input, and output the factorial of this number as a result.

### Docker File description

To build and run the application,we a are using a Dockerfile.
Based on gcc:4.9 image from dockerhub: 
* We copy the work directory into the container directory /usr/src/app, 
* We compile the C file into the executable file "server" using `RUN gcc -o server server.c`
* We start the server using `./server 9999`

### Usage
Use the docker compose file from the project root directory.

---- ONLY FOR TEST PURPOSE ----
You can build and run the C based TCP server in a standalone mode using :
`docker build -t devops-test_server .`
`docker run --name API -dt devops-test_server`


### TODO
* Optimize the way we handle the incoming message
* Try to detect any anomaly with the memory management in the code (OUTPUT expected)
* Create an Upstart script for this service, and register it in a service discovery once UP