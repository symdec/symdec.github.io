---
title: "Benchmarking d'infrastructure influxDB"
excerpt: "Analyse orientée base de données des performances d'une infrastructure influxDB pour la prédiction de séries temporelles"
header:
  image: /assets/images/influx.jpg
  teaser: assets/images/influx.jpg
---

Ce projet est de nature analytique et orienté bases de données. Il a été réalisé en binôme. Il est question de déterminer une problématique liée aux bases de données et de réaliser une implémentation technique simple permettant d'explorer le problème évoqué. Ensuite, l'accent est porté sur l'évaluation et les visualisations qui en font état, dans notre cas il s'agit de benchmarks.  

Notre sujet se centre autour d'une timeseries database, via la technologie InfluxDB, utilisée pour la prédiction de valeurs dans le temps via un modèle de Machine Learning (Adaboost). Les axes d'étude sont :
- les performances en lecture, écriture, mise à jour de la base de donnée
  - pour des requêtes sur de grands volumes de données
  - pour des écritures ponctuelles
  - pour des actions en concurrence

- les performances en terme de temps d'entraînement du modèle de Machine Learning
- la redondance des informations sur InfluxDB

Le détail de l'étude est disponible [à ce lien](https://github.com/kyn76/influxdb-benchmarking), le rapport d'étude étant présent dans le fichier `Readme.md`.  

### Date du projet :
Octobre - Novembre 2022

### Compétences générales mises en oeuvre :
- Réflexion profonde sur le choix de base de données et l'infrastructure mise en place
- Ecriture et analyse de benchmarks pour évaluer l'infrastructure / le modèle
- Démarche scientifique
- Communication écrite via le rapport et les visualisations

### Compétences techniques mises en oeuvre :
- Mise en place d'une **API Flask** : fournit une interface pour l'utilisation du modèle de prédiction
- Paramétrage d'un modèle de forecast **ARIMA**
- Création d'instances **InfluxDB**, configuration et interactions avec la base
- scripts bash et Python