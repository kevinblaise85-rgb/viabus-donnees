# Lignes de bus de Paris — données du jeu Viabus

Base de données **dérivée** des horaires officiels (GTFS) du réseau Île-de-France Mobilités.

- **Source** : Île-de-France Mobilités, via transport.data.gouv.fr
- **Jeu de données d'origine** : https://transport.data.gouv.fr/datasets/reseau-urbain-et-interurbain-dile-de-france-mobilites
- **Licence de la source** : Licence Mobilités — https://wiki.lafabriquedesmobilites.fr/wiki/Licence_Mobilit%C3%A9s
- **Extraction** : 2026-11-17
- **Contenu** : 111 lignes de bus, 1537 arrêts regroupés

## Licence de cette base

Cette base est mise à disposition sous la même licence que sa source : **Licence Mobilités** (https://wiki.lafabriquedesmobilites.fr/wiki/Licence_Mobilit%C3%A9s).
Toute réutilisation doit citer la source ci-dessus et, si elle diffuse une base dérivée, la proposer sous la même licence.

## Ce qui a été fait aux données d'origine

Seulement des choix et des regroupements, jamais d'invention :
- seules les lignes de bus sont gardées (route_type 3 et 7xx) ;
- pour chaque sens, le **parcours principal** (celui qui roule le plus de jours) ; `part` = % des trajets du sens qui le suivent ;
- les quais d'un même arrêt sont regroupés (même zone d'arrêt, ou même nom à moins de 300 m) ;
- `departs_par_heure` : départs de la ligne, heure par heure, le jour de service le plus chargé.
- seulement les lignes du cœur de la ville (au moins 50 % des passages dans le cadre, aucun arrêt à plus de 5 km) ;

## Fichiers

- `arrets.csv` : id (identifiant GTFS de l'arrêt ou de la zone), nom, commune, latitude, longitude
- `lignes.csv` : id (route_id), numéro, nom, description, type, couleur, couleur du texte, boucle
- `parcours.csv` : ligne, sens, destination, part (%), longueur (m), position, id de l'arrêt
- `departs_par_heure.csv` : ligne, puis 24 colonnes (0 h à 23 h)
- `fond_de_carte.geojson` : cours d'eau, plans d'eau, parcs et monuments affichés dans le jeu (voir ci-dessous)

## Fond de carte

Tiré d'**OpenStreetMap** (© contributeurs OpenStreetMap, licence **ODbL 1.0** — https://www.openstreetmap.org/copyright),
extrait le 2026-11-18. Cette base dérivée est mise à disposition sous la même licence (ODbL 1.0).

Seulement des choix et des simplifications, jamais d'invention : cours d'eau (rivières, canaux), plans d'eau d'au moins 1 ha,
parcs d'au moins 3 ha, contours simplifiés à 25 m, découpés au cadre de la carte du jeu et en triangles ;
au plus 12 monuments ayant une fiche Wikidata, à moins de 450 m d'un arrêt, classés par nombre d'articles Wikipédia (toutes langues).
Contenu : 224 cours d'eau, 66 plans d'eau, 120 parcs, 12 monuments
(propriété `osm` = élément OpenStreetMap d'origine).
