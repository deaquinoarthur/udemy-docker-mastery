# Docker Mastery

## Trying Out Basic Compose Commands

* CLI tool comes with Docker for Windows/Mac, but separate download for Linux.
* Not a production-grade tool but ideal for local development and test.
* Two most common commands are:
  - `docker-compose up`: setup volumes/networks and start all containers.
  - `docker-compose down`: stop all containers and remove cont/vol/net.
* If all your projects had a `Dockerfile` and `docker-compose.yml` then "new
  developer onboarding" would be:
  - `git clone github.com/some/software`
  - `docker-compose up`
