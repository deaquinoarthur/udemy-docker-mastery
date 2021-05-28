# Docker Mastery

## Docker Network DNS

- Understand how DNS is the key to easy inter-container comms
- See how it works by default with custom networks
- Learn how to use `--link` to enable DNS by default bridge network
- Containers shouldn't rely on IP's for inter-communication
- DNS for friendly names is built-in if you use custom networks
- You're using custom network right?
- This gets way easier with Docker Compose in future Section

### Forget IPs

Static IP's and using IP's for talking to container is an anti-pattern. Do your
best to avoid it.

### Docker DNS

Docker daemon has a built-in DNS server that containers use by default.

### DNS Default Names

Docker defaults the hostname to the container's name, but you can also 
set aliases.
