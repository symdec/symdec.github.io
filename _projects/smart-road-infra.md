---
title: "Simulations d'infrastructures routières intelligentes"
excerpt: "Situations routières réalistes via le simulateur SUMO, collecte de données pour forger un système multi-agents minimisant l'attente des véhicules"
header:
  image: /assets/images/road.jpg
  teaser: assets/images/road.jpg
gallery:
  - url: /assets/images/intersections.png
    image_path: assets/images/intersections.png
    alt: "Intersections et paramètres"
---

Ce projet a été réalisé dans le cadre de travaux d'une équipe de recherche orientée systèmes multi-agents (équipe SMAC du laboratoire CRIStAL).  

Il consiste en l'étude d'intersections simples du réseau routier où sont placés des feux de circulation. Via un simulateur routier nommé [SUMO](https://sumo.dlr.de/), on estime le temps d'attente moyen des usagers de chaque portion de routes pendant l'alternance régulière des feux. Ensuite, on rend ces feux réactifs aux embouteillages : ils passent au vert si un certain nombre de véhicules attendent et qu'une certaine durée s'est écoulée. 

On établit ce genre de réactivité au sein de carrefours et on récupère des métriques du simulateur afin d'estimer la durée d'attente des usagers, la taille des bouchons et d'estimer le "bonheur global" des conducteurs dans une situation réelle de ce type. On réalise de nombreuses simulations qui diffèrent selon la topologie du réseau ou les configuration des feux, et on agrège toutes ces données en séparant le comportement **statique** et **dynamique** des feux.  

{% include gallery caption="Exemple d'infrastructure étudiée : double intersection avec paramètres variables, combinés dans différentes simulations (ϕ représente l'intensité du flux de véhicules)" %}

On a pu conclure de cette étude que les feux de circulation dynamiques semblent fluidifier le trafic et donc contribuer à des usagers plus heureux. On réussit à quantifier le gain d'efficacité de circulation.  

Il s'agissait donc de travaux de modélisation et de collecte massive de données, dans le but de les exploiter plus tard via des approches de Machine Learning notamment. La finalité de l'étude dans laquelle s'inscrit ce projet est de simuler des feux communiquants dotés d'une intelligence collective afin d'optimiser au maximum le trafic et le rendre adaptatif à différents imprévus : fortes affluences, accidents, travaux etc.


### Date du projet :
Avril - Juin 2022

### Compétences mises en oeuvre :
- Démarche scientifique, décomposition du problème
- Scripts bash et Python de lancement des simulations
- Collecte de métriques du simulateur
- Nettoyage des données
- Exploitation et interprétation des résultats
- Communication écrite de la démarche et des résultats