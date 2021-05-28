# Docker Mastery

## Getting a Shell Inside Containers

**Some commands to get inside a container:**

- `docker container run -it` - start new container interactively
  `-t`, **pseudo-tty**, simulates a real terminal, like what SSH does.
  `-i`, **interactive**, keep session open to receive terminal input.
- `docker container exec -it` - run additional command in existing container
- `docker container run -it --name <name_of_container> <name_of_image> <commands> <args>`
  **e.g.** `docker container run -it --name proxy nginx bash`
  if run with `-it`, it will give you a terminal inside the running container.
