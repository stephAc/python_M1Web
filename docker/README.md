# Docker

### Quickstart

**CheatSheet**

**docker run** est une combinaison de création et de démarrage. Il crée le conteneur et le démarre.
**docker start** démarrera tous les conteneurs arrêtés. Cela inclut les conteneurs fraîchement créés.
**docker create** ajoute un conteneur au-dessus de l'image et le configure pour exécuter la commande spécifiée. L'ID du conteneur est renvoyé mais il n'a pas démarré.

- `docker version [OPTIONS]`
- `docker run [OPTIONS] IMAGE[:TAG|@DIGEST] [COMMAND] [ARG...]`
- `docker ps [OPTIONS]`
- `docker rm [OPTIONS] CONTAINER [CONTAINER...]`
- `docker start [OPTIONS] CONTAINER [CONTAINER...]`
- `docker create [OPTIONS] IMAGE [COMMAND] [ARG...]`
- `docker stop [OPTIONS] CONTAINER [CONTAINER...]`
- `docker logs [OPTIONS] CONTAINER`
- `docker exec [OPTIONS] CONTAINER COMMAND [ARG...]`
- `docker build [OPTIONS] PATH | URL | -`
- `docker kill [OPTIONS] CONTAINER [CONTAINER...]`
- `docker system prune [OPTIONS]`
- `docker image COMMAND`

### DS Sand box container

Exemple de commandes

- `docker build -t python_container .`
- `docker run -p 8000:8000 -d --name python python_container:latest`
