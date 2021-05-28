# Docker Mastery

## Docker Networks: Concepts For Private And Public Comms in Containers

**Topics:**

- Review of `docker container run -p`
- For local/dev testing, networks usually "just work"
- Quick port check with `docker container port <container_name>`
- Learn concepts of Docker Networking
- Understand how network packets move around docker

### Docker Networks Defaults

- Each container connected to a private virtual network "bridge"
- Each virtual network routes through **NAT** firewall on host IP
- All containers on a virtual network can talk to each other without -p
- Best practice is to create a new virtual network for each app:
  - network "my_web_app" for mysql and php/apache containers
  - network "my_api" for mongo and nodejs containers

### Docker Networks Cont.

- "Batteries included, but removable"
  - Defaults work well in many cases, but easy to swap out parts to customize it.
- Make new virtual networks 
- Attach containers to more then one virtual network (or none)
- Skip virtual networks and use host IP (--net=host)
- Use different Docker network drivers to gain new abilities
- and much more...
