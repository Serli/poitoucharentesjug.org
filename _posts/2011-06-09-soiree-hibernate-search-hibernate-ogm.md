---
layout: event
title:  "Soirée Hibernate Search et Hibernate OGM"
permalink: /rencontres/soiree-hibernate-search-hibernate-ogm
date: 2011-06-09 18:30:00 +0200
place: /places/pepiniere
speakers: /speakers/emmanuel-bernard
published: true
---

### Hibernate Search: Recherche full-text pour les applications d'entreprise

Hibernate Search permet à vos applications de faire des recherches à la Google sur votre base de données. Avec le montant d'informations accumulé de nos jours, rechercher et trouver rapidement les données est essentiel. Hibernate Search est un moteur de recherche full-text pour les application utilisant Hibernate Core en se focalisant sur la facilité d'utilisation et la performance.

Cette présentation parcourra les concepts de base d'Hibernate Search, comment l'utiliser et ajouter la fonction de recherche à vos applications nouvelles ou existante. Nous discuterons ensuite de fonctionnalités plus récentes comme:

 - l'indexation de masse
 - le faceting
 - l'API de configuration programmatique
 - le language de recherche plus intuitif
 - le stockage de l'index dans Infinispan

Une connaissance initiale d'Hibernate Search n'est pas nécessaire.

### Hibernate OGM: JPA pour NoSQL

PaaS (Plate-forme as a Service), Cloud, elasticité. Ces mots font le buzz ces temps-ci. Mais le vrai challenge c'est comment et où stocker vos données. Dans un data grid pour bénéficier de la scalabilité? Via une API propriétaire? Est-ce que l'on pourrait utiliser une API familière? L'objectif d'Hibernate OGM est d'explorer comment réutiliser Java Persistence et son API familière pour persister les entités dans une base de données non relationnelle.

Hibernate Object/Grid Mapper (OGM) offre une implementation JPA (manipulation d'object et requêtes JP-QL) tout en stockant et requêtant les données d'une grille clé/valeur (et d'autres approches NoSQL dans un second temps). Autrement dit, il offre une API familière tout en permettant de bénéficier des possibilités de scalabilité des data grids. Cela inclus notamment de supporter des applications JPA existantes.

Dans cette présentation, nous allons:

 - faire un survol du monde (NoSQL) et voir en quoi une API comme JPA apporte un intérêt
 - voir comment Hibernate OGM stocke les entités et les associationsdans la base clé/valeur et explorer les compromis fait
 - voir comment les requêtes JP-QL sont implémentés au dessus d'une technologie qui ne supporte pas la notion de requête (clé/valeur) et quel niveau peut être couvert
 - faire une démo d'Hibernate OGM