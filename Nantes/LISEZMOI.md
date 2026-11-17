# Lignes de bus de Nantes — données du jeu Viabus

Base de données **dérivée** des horaires officiels (GTFS) du réseau Naolib (Nantes Métropole).

- **Source** : Naolib / Nantes Métropole, via transport.data.gouv.fr
- **Jeu de données d'origine** : https://transport.data.gouv.fr/datasets/reseau-de-transports-collectifs-naolib
- **Licence de la source** : Licence Ouverte 2.0 (Etalab) — https://www.etalab.gouv.fr/licence-ouverte-open-licence/
- **Extraction** : 2026-11-17
- **Contenu** : 90 lignes de bus, 1029 arrêts regroupés

## Licence de cette base

La source est sous Licence Ouverte 2.0 (Etalab) : réutilisation libre, à condition de citer la source et la date ci-dessus.
Cette base dérivée est proposée aux mêmes conditions.

## Ce qui a été fait aux données d'origine

Seulement des choix et des regroupements, jamais d'invention :
- seules les lignes de bus sont gardées (route_type 3 et 7xx) ;
- pour chaque sens, le **parcours principal** (celui qui roule le plus de jours) ; `part` = % des trajets du sens qui le suivent ;
- les quais d'un même arrêt sont regroupés (même zone d'arrêt, ou même nom à moins de 300 m) ;
- `departs_par_heure` : départs de la ligne, heure par heure, le jour de service le plus chargé.

## Fichiers

- `arrets.csv` : id (identifiant GTFS de l'arrêt ou de la zone), nom, commune, latitude, longitude
- `lignes.csv` : id (route_id), numéro, nom, description, type, couleur, couleur du texte, boucle
- `parcours.csv` : ligne, sens, destination, part (%), longueur (m), position, id de l'arrêt
- `departs_par_heure.csv` : ligne, puis 24 colonnes (0 h à 23 h)
