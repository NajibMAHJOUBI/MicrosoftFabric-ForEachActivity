# Microsoft Fabric :  Mise en place d'un flux de contrôle itératif - Activité ForEach

Microsoft Fabric offre une plateforme unifiée visant à simplifier l'orchestration des flux de données complexes. Parmi les nombreuses activités proposées par Microsoft Fabric, l'activité ForEach offre la possibilité d'automatiser des traitements itératifs. L'activité ForEach est un conteneur de flux de travail qui exécute une série d'activités en boucle sur chaque élément d'une collection. Cela va permettre d'automatiser des traitements répétitifs sans avoir à dupliquer manuellement les mêmes opérations. Dans ce tutoriel, nous allons montrer comment maitriser cette fonctionnalité et l'utiliser efficacement. 

### Scénario

Dans ce tutoriel, nous allons interroger l'API REST [Zip Code Galore!](https://api.zippopotam.us/) qui une banque de données de codes postaux. Cette API est un service gratuit permettant de rechercher des codes postaux dans de nombreux pays et de fournir des réponses au format JSON.

- API REST : https://api.zippopotam.us/

Cette API peut être interrogée de plusieurs façon. Dans ce tutoriel, nous allons le faire avec les paramètres : 

- *country* : code du pays 
- *zipcode* : code postal

Avec ces paramètres l'interrogation de cette API se fait de la façon suivante : 

- URL avec paramètres : https://api.zippopotam.us/{country}/{zipcode}

L'ensemble du jeu de paramètres utilisées sont disponibles [ici](data/zipcode.json)

## Vidéo de démonstration

La vidé de Yotube est disponible [ici](https://youtu.be/oTpcKSEFAes).

Cette vidéo va suivre les étapes suivantes :

- [Création d'un Workspace](https://youtu.be/oTpcKSEFAes&t=32s)

- [Création d'un Lakehouse](https://youtu.be/oTpcKSEFAes&t=1m17s)

- [Création d'un Pipeline](https://youtu.be/oTpcKSEFAes&t=02m08s)

- [Ajout d'une activité ForEach](https://youtu.be/oTpcKSEFAes&t=02m51s)

- [Paramétrage du Pipeline](https://youtu.be/oTpcKSEFAes&t=03m20s)

- [Paramétrage de l'activité ForEach](https://youtu.be/oTpcKSEFAes&t=03m54s)

- [Ajout d'une activité Copy data](https://youtu.be/oTpcKSEFAes&t=04m30s)

- [Exécution du Pipeline](https://youtu.be/oTpcKSEFAes&t=08m10s)

