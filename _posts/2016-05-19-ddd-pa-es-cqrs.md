---
layout: event
title:  "DDD, P&A, ES, CQRS, ETC"
permalink: /rencontres/ddd-pa-es-cqrs
date: 2016-05-19 18:30:00 +0200
place: /places/pepiniere
speakers: /speakers/cedric-pineau,/speakers/arnaud-bailly
youtube_id: Rhp7YMcBPao
published: true
---

Parce que nous sommes tous des « fashion victims », parce que vous savez que vous ne saurez pas résister aux sirènes des micro-services, parce vous peinez déjà à justifier l'approche « full reactive » dont vous rêvez pour ce projet qui doit démarrer, nous vous proposons de prendre un peu de recul et de discuter, pour une fois, d'architecture logicielle (et de moissonner au passage quelques nouvelles munitions pour votre prochaine « buzzword battle »). 

Le « Domain-Driven Design » est un cadre conceptuel pour le développement de logiciels qui met l'accent sur l'expression directe des concepts du métier sous forme de code, dans le but de diminuer la friction entre experts métiers et informaticiens.

L'architecture « Ports And Adapters » est une démarche de structuration du code qui vise à isoler la logique métier des détails techniques de son implémentation.

« Event Sourcing » désigne un principe d'architecture, décrit par Martin Fowler, qui met au centre du monde les événements transformant l'état d'un système. L'état n'est alors rien d'autre que la suite des événements l'ayant produit à partir d'un état initial connu et précisément défini.

Le principe de « Command Query Responsibility Separation » ou CQRS est un prolongement naturel de l'Event Sourcing où l'on introduit une séparation complète des schémas de données en écriture et en lecture.

Cette présentation est un retour sur nos expériences dans la mise en œuvre de systèmes logiciels basés sur ces démarches de conception et d'architecture. Nous voulons montrer quels sont les principes de ces architectures, quels en sont les avantages tant techniques que métiers dans des cas d'utilisation concrets et comment les mettre en œuvre quels que soient les environnements techniques.
