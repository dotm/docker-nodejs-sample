# Sample Node.js application

This repository is a sample Node.js application for Docker's documentation.

## Commands Runned

- git clone https://github.com/docker/docker-nodejs-sample
- code .\docker-nodejs-sample\
- docker init
- node --version
- docker compose up --build
- docker compose up --build -d
- docker compose down

Unit test:

- docker compose run server npm run test
- docker build -t node-docker-image-test --progress=plain --no-cache --target test .

CI/CD:

- git remote set-url origin https://github.com/dotm/docker-nodejs-sample
- git push

Kubernetes:

- kubectl version --short --client
- exit
- kubectl apply -f docker-node-kubernetes.yaml
- kubectl get deployments
- kubectl get services
- kubectl delete -f docker-node-kubernetes.yaml
