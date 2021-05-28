# Docker Mastery

## Persistent Data - Bind Mounting

- Maps a host file or directory to a container file or directory
- Basically just two locations pointing to the same file(s)
- Again, skips UFS, and host files overwrite any in container
- Can't use in Dockerfile, must be at `container run`
  - `... run -v /path/in/the/host:/path/in/the/container`
