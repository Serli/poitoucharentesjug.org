# Poitou-Charentes Java User Group

Ce dépôt contient le code du site web du Poitou-Charentes JUG : https://www.poitoucharentesjug.org/

Basé sur Jekyll : https://jekyllrb.com/

## Ajout d'une rencontre

* Créer un nouveau fichier markdown dans le dossier `_posts`, en respectant la convention de nommage `<yyyy-mm-dd>-<slug>.md`, où le slug correspond au nom de la conférence en minuscule (sans accents et caractères spéciaux), avec les espaces remplacés par des tirets (Par exemple, "Introduction à MongoDB" donne `introduction-a-mongodb`).
* Renseigner les attributs suivants en haut du fichier :
  * `layout` : mettre systématiquement `event`
  * `title` :  mettre le titre de la rencontre, entre guillemets. Exemple : "Test Containers in action !"
  * `permalink` : mettre le lien permanent vers la rencontre. Exemple : `/rencontres/testcontainers-in-action`
  * `date` : mettre la date de la rencontre, au format `yyyy-mm-dd HH:MM:ss`. Exemple : `2022-06-09 18:30:00`
  * `place` : mettre le lieu de la rencontre. Exemple : `Niort Tech - 12 avenue Jacques Bujault, 79000 Niort`
  * `place_url` : mettre un lien Google Maps vers le lieu de la rencontre. Exemple : https://www.google.com/maps/place/NIORT+TECH/@46.3219417,-0.4609374,17z/data=!3m1!4b1!4m5!3m4!1s0x4807313eb267f751:0xc3ee5bdeb766eff4!8m2!3d46.3220066!4d-0.4587022
  * `speakers` : mettre le lien vers la **fiche du speaker** (lien vers le fichier du speaker dans le dossier `_speakers`, sans l'extension `.md`). Exemple : `/speakers/fedy-salah`
  * `published`: cet attribut permet de publier la rencontre. Mettre `true` pour que la rencontre soit publiée, ou bien `false` pour la laisser en "draft".
* Écrire la description de la rencontre, au format markdown, après les attributs.
  * Pour tout connaître sur le markdown : https://www.markdownguide.org/cheat-sheet/
* Et voilà !

## Fiche du speaker

Pour créer la fiche d'un speaker : 

* Créer un nouveau fichier markdown dans le dossier `_speakers`, en respectant la convention de nommage `<prenom>-<nom>.md`.
* Renseigner les attributs suivants en haut du fichier :
  * `name` : mettre le nom du speaker. Exemple : `Fedy Salah`
  * `photo` : mettre le nom du fichier de la photo du speaker, qui doit se trouver dans le dossier `assets/images/speakers`. Exemple : `fedy-salah.jpg`
  * `twitter_id` : mettre le twitter handle du speaker (sans le `@`). Exemple : `FedySalah`
* Écrire la bio du speaker, au format markdown, après les attributs.
  * Pour tout connaître sur le markdown : https://www.markdownguide.org/cheat-sheet/

## Cas particuliers 

### Cas d'une rencontre avec plusieurs speakers

S'il y a plusieurs speaker, mettre la liste des speakers **séparé par des virgules** dans l'attribut `speakers`.

Exemple : `speakers: /speakers/fedy-salah,/speakers/guillaume-soldera`

### Cas d'un speaker qui a déjà animé une rencontre et a changé de bio

Si un speaker qui a déjà animé une rencontre anime à nouveau une rencontre et a changé de bio, la bonne pratique est de créer une nouvelle fiche pour le speaker (et de ne pas modifier l'ancienne).

Pour cela, il est conseiller de compléter le nom de la fiche du speaker avec un suffixe, comme par exemple le nom de son entreprise. Par exemple pour Tug on a plusieurs fiches : 
* `/_speakers/tugdual-grall-redis.md`
* `/_speakers/tugdual-grall-mongodb.md`
