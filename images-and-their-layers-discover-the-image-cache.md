# Docker Mastery

## Images and Their Layers: Discover the Image Cache

**Topics:**

- Image layers
- Union file sytem
- `history` and `inspect` commands
- copy on write

**Review:**

- Images are made up of file system changes and metadata
- Each layer is uniquely identified and only stored once on a host
- This saves storage space on host and transfer time on push/pull
- A container is just a single read/write layer on top of image
- `docker image history` and `inspect` commands can teach us
