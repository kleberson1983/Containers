# New-Generation-Virtualization

# docker & docker-compose

# DESAFIO
Criar ambiente GKE e artifactory ou registry seguindo as instrucoes dos cards no Trello

App file ./labdocker/app.py
Modifica a app para apontar o host do redis para uma variavel de ambiente

file /labdocker/Dockerfile

Adiciona uma nova variavel de ambiente para acesso ao redis

Artifactory/Registry
Build da imagem com a modificacao feita acima

Push da image para o artifactory

GKE
dir `./manifest

Os yamls irao criar:

2 deployments (consequentemente replicaset e pods)

1 para app web e 1 para redis

2 services

1 service para a app web com type LB e 1 service para o redis (nao eh necessary definir type)

Applicar todos os yaml files com o comando abaixo

kubectl apply -f .
