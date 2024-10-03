
# __S.A.E Accompagner les utilisateurs : La carte scolaire__

## Résultats du projet

- [Feuilles de Calculs](https://docs.google.com/spreadsheets/d/1vGGsHTBB61thcOxlOQWG5S6lDTsJIJCAUaVtimA1SIk/edit?usp=sharing)
- [Carte des Collèges de la Gironde - Réussite au Brevet](https://www.google.com/maps/d/u/0/edit?mid=1ZAeDZPKG7ClccB6j2kR2H90z25_pMBQ&usp=sharing)

## Préparation

Parmi tous les sujets qui étaient disponibles, nous avons choisi de porter notre travail sur l’affectation scolaire des élèves du second degré.

Afin d’appuyer notre travail sur des données open source, nous avons créé un tableur avec les informations suivantes. La première feuille correspond aux établissements scolaires en France, la deuxième au taux de réussite au brevet en Gironde et la troisième croise les deux feuilles précédentes et reflète les établissements scolaires de la Gironde en fonction du taux de réussite au diplôme.

Pour avoir la base de notre projet, nous avons récupéré les données de tous les établissements scolaires de France sur le site ```data.gouv.com```. Le fichier Excel contenait beaucoup de bruit. Pour notre rendu, nous avions uniquement besoin des collèges généraux (publics et privés), des maisons familiales rurales et des établissements offrant une formation segpa. Deux d’entre nous ont alors nettoyé les tableurs grâce à ces trois filtres en ne gardant que :
- les lignes avec une colonne ```code_departement``` commençant par ```33```
- les lignes avec une colonne ```type_d’établissement``` contenant ```COLLEGE``` et ```MAISON FAMILIALE RURALE```

Nous avons obtenu un tableur final qui ressemblait à cela :

![excelscreenshot.PNG](ressources%2Fexcelscreenshot.PNG)

## Choix de l’axe traité

Pendant ce temps, les autres personnes du groupe ont réfléchi au choix d’un thème plus précis. Ils ont pensé à établir la carte pour afficher le secteur affilié, mais cette proposition était déjà vue et revue. 

Pour trouver une idée qui se démarque, nous avons alors mené une réflexion sur la base de cette idée : les établissements en fonction du taux de réussite au diplôme associé. Sur cette base, nous avons donc défini un objectif : **établir une carte mettant en valeur cette donnée sur l'ensemble de la Gironde.**

## Choix de l’outil utilisé :

Grâce à ChatGPT, nous avons obtenu une liste de différents sites pour réaliser des cartes.

![gptcarte.PNG](ressources%2Fgptcarte.PNG)

Parmi toutes ces propositions, nous avons retenu celle qui nous semblait la plus pertinente et qui est l’un des sites de cartographie les plus connus : Google My Maps.

## Réalisation

Pour la réalisation, voici toutes les étapes qui nous ont menées à la carte ci-dessous :
- **Étape 1** : Récolter tous les noms, informations des établissements et les nettoyer (enlever toutes les données inutiles)
- **Étape 2** : Trouver un site pour réaliser une carte et placé les premiers points de localisation avec les premières informations (nom, adresse, privé/public, filière)
- **Étape 3** : Recueillir les données complémentaires (ici, réussite au diplôme, internat, niveau d’admission) et les inclure au tableur de base
- **Étape 4** : Entrer le tableur dans ```Google My Maps```
- **Étape 5** : Établir la légende (couleur en fonction du taux de réussite) et mettre en ligne la carte sur le Github

## Difficultés rencontrées

Durant l’exercice, voici les éléments qui nous ont posé problèmes :
- **Données manquantes** : En cherchant certaines de nos données, plusieurs liens avaient l’information, mais le fichier n'était plus disponible sur le serveur. Pour d’autres, il n’y avait tout simplement pas de donnée open source, ce qui fait donc l’authenticité de la carte mais représente un manque d’information en donnée ouverte.
- **Exportation impossible** : Il nous est arrivé plusieurs fois de trouver les données qu’il nous fallait, en open source. Cependant, il était impossible de les exporter, souvent dû au format utilisé (carte, capture d’écran du tableur, etc.).
- **Croiser les tableurs** : Entre les informations manquantes et celles qui n’existent plus, les tableaux n’avaient jamais le même nombre de lignes. Il a donc fallu passer en relecture chaque nouveau tableur qui avait une donnée importante.

## Axes d’améliorations

Pour faire évoluer la carte, voici ce qu’il est possible de rajouter :
- **Secteurs** : Sur la carte, on pourrait ajouter une délimitation de secteur pour indiquer précisément les collèges de secteurs, seulement les données restent indisponibles pour le moment.
- **Transports** : De plus, l’ajout des différents points de transports pourrait être un avantage afin que les parents puissent voir de quelle manière le secteur est desservi
- **Capacité des classes** : Enfin, un paramètre qui informerait sur la capacité et le taux d’occupation des classes pourrait être pertinent.


## Sources

- [Données publique éducation national](https://defis.data.gouv.fr/defis/carte-scolaire)
- [Département de la Gironde](https://monetablissement.gironde.fr/localisation/carto)
- [L’annuaire de l’éducation](https://annuaire-education.fr/departement/gironde/033.html?tout=oui&statut_public=oui&statut_prive=oui&type_college=oui&type_erea=oui)
- [Ministère de l’éducation nationale](https://www.education.gouv.fr/panorama-scolaire#:~:text=Ce%20panorama%20synth%C3%A9tique%20des%20%C3%A9tablissements%20vise%20%C3%A0%20rendre%20compte%20de)
- [Indicateurs de valeur ajoutée des collèges](https://www.data.gouv.fr/fr/datasets/indicateurs-de-valeur-ajoutee-des-colleges/)
- [MFR du Blayais](https://www.mfrblaye.fr/)
- [Maison Familiale Rurale de l'Entre-Deux-Mers – Établissement scolaire d’enseignement agricole en alternance (Sauve Majeure – Gironde)](https://www.mfr-entredeuxmers.fr/)
- [MFR DE VAYRES - Formations par alternance entre Bordeaux et St Emilion](https://mfr-vayres.fr/)
