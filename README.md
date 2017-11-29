# Docker angular-serve

## Description
This is a container that run a server for your angular project

## Version 1.0.0
First version of docker image to help run a angular project on a server, based on Angular CLI image.

## Usage
You can find the image on docker cloud ready to use: [jcbjulio/angular-serve](https://cloud.docker.com/swarm/jcbjulio/repository/docker/jcbjulio/angular-serve) [(source)](https://github.com/jcbjulio/angular-serve)

### Run
`docker run -v <local_project_full_path>:/app -p 80:4200 jcbjulio/angular-serve`
### Example
`docker run -v ~/angularProjects/my-app:/app -p 80:4200 jcbjulio/angular-serve`

This will mount your project (which should be allready installed) inside the container at location `/app` and run the server using it.
The server will run inside the docker on port 4200 and will expose to a choosen port when you run the container. 
In our example above it will be accessable on the por 80 on your local computer.

## Parent project
### [jcbjulio/angular-cli](https://cloud.docker.com/swarm/jcbjulio/repository/docker/jcbjulio/angular-cli) [(source)](https://github.com/jcbjulio/angular-cli)
To use manually the angular-cli, you can use this base image.

## Other projects
### [jcbjulio/angular-install](https://cloud.docker.com/swarm/jcbjulio/repository/docker/jcbjulio/angular-install) [(source)](https://github.com/jcbjulio/angular-install)
To use it just to `npm install` an already created project for angular, you can use this especific image.
