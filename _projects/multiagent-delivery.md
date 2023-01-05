---
title: "Collecte et livraison via système multi-agents"
excerpt: "Implémentation multi-agents de résolution d'un problème classique de logistique en Python orienté objet, avec interface graphique Tkinter"
header:
  image: /assets/images/delivery.jpg
  teaser: assets/images/delivery.jpg
---

Ce projet réalisé en binôme vise à résoudre un problème de logistique : la collecte de colis par des livreurs et leur acheminement vers un dépôt. Chaque colis possède une masse donnée, chaque livreur possède une force donnée. Ainsi, certains colis nécessitent que des livreurs forment une équipe pour les transporter. L'objectif visé est d'acheminer tous les colis en minimisant l'effort de tous les livreurs, l'approche est donc utilitariste (elle maximise le bonheur moyen).  

Nous avons implémenté différentes stratégies de collecte/livraison :
- La stratégie aléatoire où les déplacements et actions des livreurs sont erratiques et non déterministes, il s'agit de la stratégie "témoin", nécessairement sous-optimale.
- La stratégie d'attribution aléatoire de colis : chaque livreur ou équipe vise un colis aléatoire et l'achememine vers un dépôt aléatoire.
- La stratégie d'attribution au plus proche : chaque livreur ou équipe vise le colis le plus proche qu'il/elle peut porter et l'achemine vers le dépôt le plus proche. Cela semble être l'approche optimale. Cependant il existe un moyen d'améliorer cette stratégie.
- La stratégie d'attribution au plus proche avec échange de tâche : même démarche que la précédente mais les livreurs sont en mesure de s'échanger des colis si cette inversion minimise l'effort des deux partis.

Le problème a été abordé selon le paradigme objet, chaque élément de la simulation est un objet, notamment les actions réalisées par les livreurs (déplacement, collecte, dépôt, échange, agrégation). L'abstraction du problème en classes et sous-classes a été hardue mais a ensuite permis une implémentation efficace.  

L'effort des livreurs est quantifié au cours des simulations, ce qui a permis d'évaluer les différentes stratégies et de conclure qu'elles sont de plus en plus efficaces à mesure qu'on descend dans la liste ci-dessus.

### Date du projet :
Octobre - Novembre 2022

### Compétences mises en oeuvre :
- Modélisation et implémentation ex nihilo
- Travail en équipe : pair programming
- Logique et vision multi-agents
- Implémentation en Python orienté objet, structuré (héritage, abstraction)
- Interface graphique Tkinter
- Création de métriques et évaluation des stratégies de résolution