# node.js-docker-example
This project is a reference to create a docker boilerplate for a node js with express.

## Project Setup
There are two ways to follow this process. The first one is to clone this repository as your starting project and modify the docker file according to your needs. The second way is to create your own node js project and reference the docker file created in this repository to setup in your own project.
<br/>

## Build Docker Image

1. Open terminal and navigate to your project or repository
2. Enter the following command to build an image. (The docker file must be in the root of your project)

    **Example**

    `docker build -t user-service-api:latest .`

    **Command**

    `docker build -t [image name]:[image tag] [current directory (.) or path to the directory (C:/path)]`
3. By building the project, a image will be created. To run the image aka container, enter the following command

    **Example**

    `docker run --name user-api -d -p 3000:3000 user-service-api:latest`

    **Command**

    `docker run --name [name for container] -d -p 3000:3000 [image name]:[image tag]`
4. After executing the above command, an instance of your image will run at port 3000.
