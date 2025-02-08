---
title: "Analyse de sentiments sur Twitter"
excerpt: "Analyses syntaxiques et sémantiques de tweets aﬁn d'extraire le sentiment global lié à un thème sur le réseau social"
header:
  image: /assets/images/sentwitter.jpg
  teaser: assets/images/sentwitter.jpg
---

Ce projet orienté Natural Language Processing (NLP) a été une introduction au domaine au début du master (en binôme). Il s'agissait d'utiliser l'API de Twitter afin de récupérer des tweets et de les classifier comme étant positifs, négatifs ou neutres dans le sentiment véhiculé. Il s'agissait de construire à la main un dataset d'entraînement avec quelques centaines de tweets étiquetés selon le sentiment dégagé, puis d'appliquer des modèles de Machine Learning de plus en plus avancés afin de prédire le sentiment global sur un certains nombre de tweets d'un nouveau thème.  

Les modèles étudiés pour cela :
- Classifieur naïf par dictionnaires (mots clé positifs / négatifs)
- K plus proches voisins (KNN)
- Probabiliste, guidé par les statistiques : Naive Bayes appliqué avec un modèle unigramme et bigramme

Nous avons également mis en place des scoreurs de ces différents modèles.  

Ce projet a été réalisé en Java, les algorithmes des modèles ci-dessus ont donc été écrit dans un paradigme purement objet.  

Le code source n'est pas rendu disponible mais les détails de la démarche et des résultats sont visibles dans le rapport [à ce lien](https://github.com/symdec/twitter-sentiment-report/blob/main/Twitter-Feelings-Report.pdf).

### Date du projet :
Septembre - Novembre 2021

### Compétences mises en oeuvres :
- Compréhension de modèles de machine learning basiques en NLP, car implémentation soi-même
- Intereaction avec une API de réseau social
- Programmation orientée objet
- Preprocessing de langage naturel pour donner au texte une forme adaptée aux algorithmes (tokenizer, filtres etc.)
- Classification : par dictionnaire, KNN, Naive Bayes
- Evaluation de modèles et d'hyperparamètres

