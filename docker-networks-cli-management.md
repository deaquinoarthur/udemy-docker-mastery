# Docker Mastery

## Docker Networks: CLI Management

- Show networks: `docker network ls`
- Inspect a network: `docker network inspect`
- Create a network: `docker network create --driver`
- Attach a network to a container: `docker network connect`
- Detach a network from container: `docker network disconnect`

- `--network bridge` - Default docker virtual network which is NAT'ed behind the
host IP.
- `--network host` - It gains performance by skipping virtual networks but
sacrifices security of container mode.
- `--network none` - Removes **eth0** and only leaves you with localhost interface 
in container.
- `docker network create <network_name>` - Spawns a new virtual network for you to
attach containers to.

- **network driver:** - Built-in or 3rd party extensions that give you virtual
  network features.

### Docker Networks: Default Security

- Create your apps so frontend/backend sit on same Docker network
- Their inter-communication never leaves host
- All externally exposed ports closed by default
- You must manually expose via `-p` which is better default security
- This gets even better later with Swarm and Overlay networks
