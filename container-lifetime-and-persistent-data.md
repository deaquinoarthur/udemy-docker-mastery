# Docker Mastery

## Container Lifetime & Persistent Data

**Section Overview**

- Defining the problem of persistent data
- Key concepts with containers: **immutable**, **ephemeral**
- Learning and using **Data Volumes**
- Learning and using **Bind Mounts**
- Assignments

**Concepts**

- Containers are usually **immutable** and **ephemeral**
- "immutable infrastructure": only re-deploy containers, never change
- This is the ideal scenario, but what about databases, or unique data?
- Docker gives us features to ensure these "separation of concerns"
- This is known as "persistent data"
- Two ways: Volumes and Bind Mounts
- **Volumes:** make special location outside of container UFS
- **Bind Mounts:** link container path to host path
