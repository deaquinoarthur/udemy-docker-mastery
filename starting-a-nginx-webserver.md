# Docker Mastery

## Starting a Nginx Webserver

**This Lecture:**

- image vs. container
- run/stop/remove containers
- check container logs and processes

### Image vs. Container

* An Image is the application we want to run (libraries, 
  source code, binaries).
* A Container is an instance of that image running as a process.
* You can have many containers running off the same image.
* In this lecture our image will be the Nginx web server.
* Docker's default image "registry" is called Docker Hub
  (hub.docker.com)
  
**Running the first container:**

`docker container run --publish 80:80 <images_name>`

e.g. `docker container run --publish 80:80 nginx`

1. Downloaded image 'nginx' from Docker Hub.
2. Started a new container from that image.
3. **--publish 80:80**: Opened port 80 on the host IP.
4. Routes that traffic to the container IP, port 80.

**Running the container on the background:**

`docker container run --publish 80:80 --detach <images_name>`

e.g. `docker container run --publish 80:80 --detach nginx`

**Stopping container:**

`docker container stop <containers_id>`

e.g. `docker container stop e3bd406b3bf3`

**Listing containers:**

`docker container ls`

**Listing all the containers (including stopped ones):**

`docker container ls -a`

**Starting a named container:**

`docker container run --publish 80:80 --detach --name <containers_name> <images_name>`

e.g. `docker container run --publish 80:80 --detach --name webhost nginx`

**Showing the container's log:**

`docker container logs <containers_name>`

e.g. `docker container logs webhost`

**Looking the processes running inside a container:**

`docker container top <containers_name>`

e.g. `docker container top webhost`

**Removing multiple stopped containers:**

`docker container rm <container1_id> <container2_id>`

e.g. `docker container rm 32g as8`

**Removing multiple containers (even the running ones):**

Using the flag `-f` we are forcing the container to be removed,
even if it is running.

`docker container rm -f <container1_id> <container2_id>`

e.g. `docker container rm -f 32g as8`
