# Docker Mastery

## What happens in 'docker container run'

1. Looks for the image locally in image cache, doesn't find anything.
2. Then looks in remote image repository (defaults to Docker Hub)
3. Downloads the latest version (nginx:latest by default)
4. Creates a new container based on the image and prepares to start
5. Gives it a **virtual IP** on a private network inside **Docker Engine**
6. Opens up port 80 on host and forwards to port 80 in container
7. Starts container by using the CMD in the image Dockerfile
