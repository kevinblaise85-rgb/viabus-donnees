# Lignes de bus de Toulouse — données du jeu Viabus

Base de données **dérivée** des horaires officiels (GTFS) du réseau Tisséo (Toulouse Métropole).

- **Source** : Tisséo / Toulouse Métropole, via transport.data.gouv.fr
- **Jeu de données d'origine** : https://transport.data.gouv.fr/datasets/tisseo-reseau-transport-urbain-toulousain
- **Licence de la source** : ODbL (Open Database License) — https://opendatacommons.org/licenses/odbl/
- **Extraction** : 2026-11-17
- **Contenu** : 119 lignes de bus, 1815 arrêts regroupés

## Licence de cette base

Cette base est mise à disposition sous la même licence que sa source : **ODbL (Open Database License)** (https://opendatacommons.org/licenses/odbl/).
Toute réutilisation doit citer la source ci-dessus et, si elle diffuse une base dérivée, la proposer sous la même licence.

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
