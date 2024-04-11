# DevOps - Monitoring et centralisation des logs

## Description

- Déployer une stack Elastic pour centraliser les logs de nos conteneurs Docker
- Consultation des logs avec Kibana
- Déploiement d'un service de monitoring avec Prometheus
- Visualisation des Dashboards avec Grafana

## Technos utilisés :

- ElasticSearch
- Kibana
- Prometheus
- Grafana
- Docker
- DockerCompose

## Utilisation

Avant de up le docker-compose, il est nécéssaire de lancer dans le dossier racine "myworks" ces commandes, qui permettent de charger le module Filebeat d'elasticsearch qui permettra facilement de centraliser tous les logs de nos différents conteneurs Docker.

- curl -L -O https://raw.githubusercontent.com/elastic/beats/7.10/deploy/docker/filebeat.docker.yml

- mv filebeat.docker.yml filebeat.yml

- sudo chown root filebeat.yml

- sudo chmod go-w filebeat.yml
