# Read Me

## Problem:
Using docker-compose for container orchestration, establish https communication between an MVC UI and a .NET Web API each in separate containers.

## Solution:
1. Remove the `EXPOSE 80` and `EXPOSE 443` from each Dockerfile
2. In docker-compose.yml add ports to each service. I added `- "49161:443"` to my UI service and `- "49162:443"` to my API service.
3. Remove ports sections from each service in docker-compose.override.yml

### *Note:
I'm not 100% satisfied with this solution. [Networking in Compose](https://docs.docker.com/compose/networking/) promises a cleaner solution to this problem. Seems like either way, I will ultimately need to store the hostname with its port (i.e. localhost:49162) in some kind of environment variable. 
