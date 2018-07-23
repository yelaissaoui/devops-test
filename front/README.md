### Description
This repository contains a single page app, its React based, the skelton of the app was generate using : https://github.com/facebookincubator/create-react-app


### Docker File description

To build and run the application,we a are using a Dockerfile.
Based on node:8 image from dockerhub: 
* We copy the work directory into the container directory /usr/src/app, 
* We install the prerequisites running `npm i`
* We run the tests using `mocha`
* We build the app using `npm run build`
* We start the server using `npm run start`

### Usage
Use the docker compose file from the project root directory.

---- ONLY FOR TEST PURPOSE ----
You can build and run the node app in a standalone mode using :
`docker build -t devops-test_front .`
`docker run --name API -dt devops-test_front`


### FYI
API Endpoint is hardcoded in `src/App.js` Line 5, I don't think this is a good practice, do you ?

### Deployment
--DONE-- This application needs to be deployed behind a web server, preferred Nginx
