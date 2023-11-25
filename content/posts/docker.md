---
title: "Docker"
date: 2023-04-21T21:15:02+02:00
modified: 2023-11-25T09:19:00+02:00s
draft: false
tags: ["linux", "cheat-sheet"]

---

## Docker

```bash
docker pull : Récupérer une image depuis un registre
```

```bash
docker run :

- p 8080:8080
- rm : Supprimer le conteneur à la fin de son exécution
- it : Interactif
- v $(pwd):/src
- d : Détaché
- e : Variables d’environnement
```

```bash
docker run -p 8080:8080 -rm -it -v $(pwd):/src -d -e NODE_ENV=production nom_de_l_image
```

docker run => docker create + docker start

docker create id_de_l_image

docker start id_du_conteneur

docker stop id_du_conteneur

docker restart id_du_conteneur

docker rm id_du_conteneur

docker rmi id_de_l_image

docker exec -it id_du_conteneur bash

docker logs id_du_conteneur

docker stats

docker system prune : Supprimer tous les conteneurs, images, volumes et réseaux non utilisés

docker system prune -a : Supprimer tous les conteneurs, images, volumes et réseaux (même utilisés)

docker system df : Afficher l’espace disque utilisé par les images et les conteneurs

docker images : Afficher les images

```
docker ps -a
CONTAINER ID : Identifiant unique du conteneur
IMAGE : Image utilisée pour créer le conteneur
COMMAND : Commande exécutée au lancement du conteneur
CREATED : Date de création du conteneur
STATUS : Statut du conteneur
PORTS : Ports exposés par le conteneur
NAMES : Nom du conteneur
```

## docker-compose

docker build : Construire une image à partir d’un Dockerfile

docker build -t nom_de_l_image .

docker-compose run --rm hugo --help

Docker Compose : yaml
Dockerfile :

```bash
    FROM node:12-alpine
    RUN apk add --no-cache python2 g++ make
    WORKDIR /app
    COPY . .
    RUN yarn install --production
    CMD ["node", "src/index.js"]
    EXPOSE 3000
```

Dockerfile :

```yaml
docker-compose.yml :
    version: '3'
    services:
    web:
        build: .
        ports:
        - "3000:3000"
        volumes:
        - .:/app
        - /app/node_modules
    db:
        image: mongo
        ports:
        - "27017:27017"
```

docker-compose up : Lancer les conteneurs

docker-compose up -d

docker-compose down : Arrêter les conteneurs

## docker maintenance

docker system prune

docker system prune -a

docker system df

docker volume prune

docker volume ls

docker volume rm id_du_volume

docker volume rm $(docker volume ls -q)

sudo systemctl status docker

sudo systemctl start docker

sudo systemctl stop docker

sudo systemctl restart docker

sudo systemctl enable docker

sudo systemctl disable docker

sudo systemctl status docker

## docker configuration

<https://www.docker.com/products/docker-desktop/>
<https://docs.docker.com/engine/install/ubuntu/>

```bash
sudo apt-get remove docker docker-engine docker.io containerd runc
```

```bash
sudo apt update
```

```bash
sudo apt-get install \
    ca-certificates \
    curl \
    gnupg
```

```bash
sudo install -m 0755 -d /etc/apt/keyrings
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /etc/apt/keyrings/docker.gpg
sudo chmod a+r /etc/apt/keyrings/docker.gpg
```

```bash
echo \
  "deb [arch="$(dpkg --print-architecture)" signed-by=/etc/apt/keyrings/docker.gpg] https://download.docker.com/linux/ubuntu \
  "$(. /etc/os-release && echo "$VERSION_CODENAME")" stable" | \
  sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
```

```bash
sudo apt-get update
```

```bash
sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
```

```bash
ls -l /var/run/docker.sock :  check the permissions
```

```bash
sudo chmod 666 /var/run/docker.sock
```

```bash
sudo chown root:docker /var/run/docker.sock
```

```bash
sudo usermod -aG docker $USER : Add user to docker group
```

### ajouter les droits docker à l'utilisateur courant

```bash
sudo groupadd docker
```

```bash
sudo usermod -aG docker $USER
```

```bash
newgrp docker
```

```bash
docker run hello-world
```
