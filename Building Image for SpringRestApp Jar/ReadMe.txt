Here we have copied the jar --RestApp-0.0.1-SNAPSHOT.jar-- from SpringRestApp\RestApp\target

Then created the Docker File -- Dockerfile

Building the DockerFile : docker build -t <name> . 
                          docker build -t dockjar .

Running the created Image : docker run -d -p <hostmachineport>:<containerport> -it --name <containername> <imageid/name>
                            docker run -d -p 8080:8084 -it --name jarcont dockjar

Once container is started, we can view the application on web browser:
http://localhost:8080/

as per Our Project, you will get below output as mentioned:

http://localhost:8084/
Welcome to RestApp, Application is running

http://localhost:8084/hello
Hello World!

http://localhost:8084/hello?name=shivani
Hello shivani!

http://localhost:8084/test1
This is test1
