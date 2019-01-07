# Gitea Docker Swarm Setup
Use Gitea in a Docker Swarm in the Hetzner Cloud

## Requierments

- Hetzner Cloud Account
- A Docker Swarm
- This [plugin](https://github.com/costela/docker-volume-hetzner) enabled and configured on all nodes / managers


## Setup
- Change domain.com to your domain
- Deploy the two stack files from you manager node:   
```docker stack deploy --compose-file gita.stack gitea```  
```docker stack deploy --compose-file traefik.stack traefik```
