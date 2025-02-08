---
title: "Tymon"
excerpt: "Projet personnel : extracteur étymologique basé sur Wikitionnaire, centralisation des recherches d'étymologie de mots français et anglais"
header:
  image: /assets/images/tymon.jpg
  teaser: assets/images/tymon.jpg
gallery:
  - url: /assets/images/tymon_example.png
    image_path: assets/images/tymon_example.png
    alt: "Exemple d'utilisation de Tymon"
---

Tymon (dérivé du terme *étymon*) est un petit programme personnel qui répond à une problématique à laquelle j'ai pu être confronté. Etant de nature curieuse et plutôt fan d'étymologie, il m'arrive souvent de me demander d'où viennent certains mots. Une recherche Google suffit, mais si je décide de chercher l'origine d'autres mots, il faut changer de page encore et encore. Sans compter le fait que d'autres informations sur le mot apparaissent en plus de son étymologie.  

Je me suis donc mis à la recherche d'un agrégateur étymologique, mais n'en trouvant aucun, j'ai décidé de le créer moi même. Il me suffit désormais d'ouvrir un terminal, d'invoquer ma commande suivie du mot cherché, avec éventuellement une option si je veux chercher l'origine de mots en anglais. J'ai prévu d'étendre davantage l'outil pour notamment rajouter d'autres langues et réaliser une recherche complémentaire en cas d'échec.


### Fonctionnement :
Le programme, écrit en Python, est basé sur un requêtage du site Wikitionnaire (Wiktionary) via cURL. Une fois le HTML de la page récupéré, je navigue à l'intérieur de cette arborescence pour trouver la section étymologique et extraire le texte sur l'origine du mot. Il suffit ensuite de ne retourner que ces informations à l'utilisateur.

Je travaille actuellement sur une extension propulsée par NLP et permettant une recherche complémentaire d'étymologie dans le cas où la requête au Wikitionnaire est infructueuse. Elle récupèrerait le contenu des premières pages / résultats suite à une recherche internet, puis utiliserait un modèle de Question Answering d'HuggingFace afin d'extraire l'étymologie quelque soit la manière dont elle est explicitée dans la page.

{% include gallery caption="Exemple d'utilisation de Tymon" %}

[Le dépôt GitHub de l'outil est disponible ici.](https://github.com/symdec/tymon)

### Date du projet :
Octobre 2022 - 2023

### Compétences mises en oeuvre :
- Utilisation d'API en Python
- Utilisation de modèles de NLP (QA) pré-entraînés
- Navigation dans une arborescence HTML, via des librairies Python
- Publication de code open-source (GitHub, effort sur la communication du code)
- Résolution libre d'une problématique, démarche personnelle
