# Turtl-dev-environment

Ce projet permet de déployer rapidement un environnement de dévelopement pour l'application de prise de notes [Turtl](https://turtl.it/)

Tous les composants de ce projet sont embarqués dans des conteneurs docker.

# Organisation du projet

* `js` un sous-module git pointant vers un fork du cœur de turtl. C'est ici que les modifications se font
* `turtl-docker` un sous-module git pointant vers un conteneur embarquant l'API pour persister les données
* `docker-compose.yml` permettant de lancer le tout

# En vrac

* `turtl-docker` penser à modifier la valeur de `enabled-cors-resources` dans `config.footer` et `config.lisp` pour permettre les appels depuis le navigateur depuis un autre domaine
