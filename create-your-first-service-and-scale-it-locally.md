# Docker Mastery

`docker swarm init`, what just happens?

* Lots of PKI and security automation
  * Root Signing Certificate created for our Swarm 
  * Certificate is issued for first manager node
  * Join tokens are created
* Raft database created to store root CA, configs and secrets 
  * Encrypted by default on disk (1.13+)
  * No need for another key/value system to hold orchestration/secrets
  * Replicates logs amongst Managers via mutual TLS in "control plane"

**Creating an alpine service:**
`docker service create alpine ping 8.8.8.8`

**Listing the services:**
`docker service ls`

**Listing the containers running on a service:**
`docker service ps <name_of_the_service>`

**Adding more replicas to a service:**
`docker service updated <id_of_the_service> --replicas <desired_number>`
