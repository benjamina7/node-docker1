# node-docker1
simple test of node runnning in docker container

### NOTES:
    * app's index.js sets the port to be used for itself as 8081
    * dockerfile says to expose this app from the container as port 8082
    * in run command below, we map the exposed container port 8082 to the apps running port 8081

`docker build -t node-docker .`

`docker run -p 8082:8081 node-docker`

**now access app from http://localhost:8082**