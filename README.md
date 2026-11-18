# Données ouvertes du jeu Viabus

Le jeu Roblox **Viabus** utilise les vraies lignes de bus de villes d'Europe. Voici les bases dérivées utilisées
par le jeu, ville par ville, chacune **sous la licence de sa source** (voir le LISEZMOI de chaque dossier).

## Lignes de bus et fond de carte (villes françaises)

Lignes tirées des horaires officiels publiés sur transport.data.gouv.fr ; fond de carte d'OpenStreetMap (ODbL).

| Ville | Lignes | Arrêts | Licence | Source |
|---|---|---|---|---|
| [Lille](Lille/) | 154 | 1519 | Licence Ouverte 2.0 (Etalab) | ilévia / Métropole Européenne de Lille, via transport.data.gouv.fr |
| [Rennes](Rennes/) | 153 | 829 | ODbL (Open Database License) | STAR / Rennes Métropole, via transport.data.gouv.fr |
| [Toulouse](Toulouse/) | 119 | 1815 | ODbL (Open Database License) | Tisséo / Toulouse Métropole, via transport.data.gouv.fr |
| [Marseille](Marseille/) | 115 | 1285 | Licence Ouverte 2.0 (Etalab) | RTM / Métropole Aix-Marseille-Provence, via transport.data.gouv.fr |
| [Bordeaux](Bordeaux/) | 119 | 1991 | Licence Ouverte (Etalab) | TBM / Bordeaux Métropole, via transport.data.gouv.fr |
| [Nantes](Nantes/) | 90 | 1029 | Licence Ouverte 2.0 (Etalab) | Naolib / Nantes Métropole, via transport.data.gouv.fr |
| [Strasbourg](Strasbourg/) | 40 | 543 | Licence Ouverte 2.0 (Etalab) | CTS - Compagnie des Transports Strasbourgeois, via transport.data.gouv.fr |
| [Nice](Nice/) | 103 | 1582 | Licence Ouverte 2.0 (Etalab) | Lignes d'Azur / Métropole Nice Côte d'Azur, via transport.data.gouv.fr |
| [Montpellier](Montpellier/) | 39 | 601 | ODbL (Open Database License) | TaM / Montpellier Méditerranée Métropole, via transport.data.gouv.fr |
| [Grenoble](Grenoble/) | 124 | 965 | ODbL (Open Database License) | TAG / SMMAG (Syndicat Mixte des Mobilités de l'Aire Grenobloise), via transport.data.gouv.fr |
| [Paris](Paris/) | 111 | 1537 | Licence Mobilités | Île-de-France Mobilités, via transport.data.gouv.fr |

## Fond de carte seulement (autres pays)

Cours d'eau, plans d'eau, parcs et monuments tirés d'OpenStreetMap (© contributeurs OpenStreetMap, ODbL 1.0).

| Ville | Pays | Cours d'eau | Plans d'eau | Parcs | Monuments | Extraction |
|---|---|---|---|---|---|---|
| [Luxembourg](Luxembourg/) | LU | 38 | 15 | 21 | 12 | 2026-11-18 |
| [Esch-sur-Alzette](Esch/) | LU | 50 | 13 | 9 | 12 | 2026-11-18 |
| [Charleroi](Charleroi/) | BE | 54 | 36 | 21 | 12 | 2026-11-18 |
| [Liège](Liege/) | BE | 49 | 23 | 20 | 12 | 2026-11-18 |
| [Namur](Namur/) | BE | 33 | 11 | 5 | 7 | 2026-11-18 |
| [Mons](Mons/) | BE | 51 | 33 | 14 | 7 | 2026-11-18 |
| [Amsterdam](Amsterdam/) | NL | 2572 | 80 | 108 | 12 | 2026-11-18 |
| [Rotterdam](Rotterdam/) | NL | 1072 | 80 | 120 | 12 | 2026-11-18 |
| [La Haye](LaHaye/) | NL | 569 | 80 | 117 | 12 | 2026-11-18 |
| [Utrecht](Utrecht/) | NL | 785 | 80 | 67 | 12 | 2026-11-18 |
| [Eindhoven](Eindhoven/) | NL | 71 | 80 | 35 | 12 | 2026-11-18 |
| [Madrid](Madrid/) | ES | 189 | 43 | 120 | 12 | 2026-11-18 |
| [Valence](Valence/) | ES | 499 | 69 | 41 | 12 | 2026-11-18 |
| [Berlin](Berlin/) | DE | 383 | 80 | 120 | 12 | 2026-11-18 |
| [Hambourg](Hambourg/) | DE | 763 | 80 | 120 | 12 | 2026-11-18 |
| [Munich](Munich/) | DE | 322 | 80 | 120 | 12 | 2026-11-18 |
| [Cologne](Cologne/) | DE | 66 | 80 | 120 | 12 | 2026-11-18 |
| [Francfort](Francfort/) | DE | 134 | 80 | 117 | 12 | 2026-11-18 |
| [Zurich](Zurich/) | CH | 78 | 35 | 17 | 12 | 2026-11-18 |
| [Genève](Geneve/) | CH | 219 | 48 | 90 | 12 | 2026-11-18 |
| [Bâle](Bale/) | CH | 127 | 44 | 27 | 12 | 2026-11-18 |
| [Berne](Berne/) | CH | 40 | 44 | 7 | 12 | 2026-11-18 |
| [Lausanne](Lausanne/) | CH | 93 | 7 | 11 | 12 | 2026-11-18 |

Jeu non officiel, sans lien avec ces réseaux. Aucun logo ni marque d'opérateur.

## Licences

Chaque dossier porte la licence de sa source (détails dans son `LISEZMOI.md`) :
- **Licence Ouverte / Open Licence (Etalab)** — https://www.etalab.gouv.fr/licence-ouverte-open-licence/
- **ODbL 1.0 (Open Database License)** — https://opendatacommons.org/licenses/odbl/1-0/ (Rennes, Toulouse, Montpellier, Grenoble)
- **Licence Mobilités** (Île-de-France Mobilités) — Paris
- **Fond de carte** (`fond_de_carte.geojson` de chaque ville : cours d'eau, plans d'eau, parcs, monuments) : tiré d'**OpenStreetMap**, © contributeurs OpenStreetMap, **ODbL 1.0** — https://www.openstreetmap.org/copyright — et proposé sous la même licence

Les fichiers sont regénérés à chaque mise à jour des horaires officiels.
