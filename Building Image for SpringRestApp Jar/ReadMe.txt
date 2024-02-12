Here we have copied the jar --RestApp-0.0.1-SNAPSHOT.jar-- from SpringRestApp\RestApp\target

Then created the Docker File -- Dockerfile

Building the DockerFile : docker build -t <name> . 
                          docker build -t dockjar .

Running the created Image : docker run -d -p <hostmachineport>:<containerport> -it --name <containername> <imageid/name>
                            docker run -d -p 8080:8084 -it --name jarcont dockjar
