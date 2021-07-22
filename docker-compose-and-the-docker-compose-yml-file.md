# Docker Mastery

## Docker Compose and the docker-compose.yml file

* Why: configure relationships between containers
* Why: save our docker container run settings in easy-to-read file
* Why: create one-liner developer environment startups
* Comprised of 2 separeted but related things:
  1. YAML-formatted file that describes our solution options for:
    * containers
    * networks
    * volumes
  2. A CLI tool `docker-compose` used for local dev/test automation with those
     YAML files

### docker-compose.yml

* Compose YAML format has it's own versions: 1, 2, 2.1, 3, 3.1
* YAML file can be used with `docker-compose` for local docker automation or...
* With `docker` directly in production with Swarm (as of v1.13)
* `docker-compose --help`
* `docker-compose.yml` is default filename, but any can be used with `docker-compose -f`
