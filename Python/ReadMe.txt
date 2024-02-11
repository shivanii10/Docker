How to run a Python Program using Docker:

- check docker is proprtly installed using docker run hello-world.
You will get below output:
---------------------------------------------------------------------------------------
C:\Users\Shivani>docker run hello-world

Hello from Docker!
This message shows that your installation appears to be working correctly.

To generate this message, Docker took the following steps:
 1. The Docker client contacted the Docker daemon.
 2. The Docker daemon pulled the "hello-world" image from the Docker Hub.
    (amd64)
 3. The Docker daemon created a new container from that image which runs the
    executable that produces the output you are currently reading.
 4. The Docker daemon streamed that output to the Docker client, which sent it
    to your terminal.

To try something more ambitious, you can run an Ubuntu container with:
 $ docker run -it ubuntu bash

Share images, automate workflows, and more with a free Docker ID:
 https://hub.docker.com/

For more examples and ideas, visit:
 https://docs.docker.com/get-started/

---------------------------------------------------------------------------------------

- create a Python program, here main.py.
- create dockerfile, here Dockerfile.
- both the files should be same directory.
- open cmd.
- build docker image : docker build -t <img-name> .
                       docker build -t py-image .
- view docker images: docker images 
                      REPOSITORY    TAG       IMAGE ID       CREATED          SIZE
                      py-image    latest    af8860dcd6c0   27 seconds ago   470MB
- To run the docker image: docker run <img-name>,
                           docker run py-image
                           Output: Trial (Python fil will be executed)
