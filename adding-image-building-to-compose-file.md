# Docker Mastery

## Adding Image Building to Compose File

### Using Compose to Build

- Compose can also buid your custom images.
- Will build them with `docker-compose up` if not found in cache.
- Also rebuild with `docker-compose build`
- Great for complex builds that have lots of vars or build args.
