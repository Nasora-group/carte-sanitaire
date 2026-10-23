# Carte sanitaire du Sénégal

Carte interactive construite à partir du fichier HTML initial de Dakar, en conservant sa présentation SVG, ses couleurs, ses onglets et son panneau d'informations.

## Couverture

- **14 régions administratives** affichées dans la vue nationale.
- Chaque région peut être sélectionnée pour zoomer.
- La vue **Dakar (détail)** conserve la carte initiale des communes et ses structures connues.
- Les contours des 14 régions sont intégrés directement dans `index.html` : la géométrie de la carte nationale ne dépend pas d'un appel API externe.
- Les points complémentaires des structures de santé sont récupérés en ligne depuis OpenStreetMap via Overpass. Leur chargement nécessite une connexion et peut être indisponible temporairement.

## Utilisation

- Dépôt : https://github.com/Nasora-group/carte-sanitaire
- Fichier HTML : https://github.com/Nasora-group/carte-sanitaire/blob/main/index.html
- Pour télécharger le HTML : https://raw.githubusercontent.com/Nasora-group/carte-sanitaire/main/index.html

Télécharger `index.html` puis l'ouvrir dans un navigateur. Les contours régionaux sont intégrés au fichier ; les structures complémentaires OpenStreetMap nécessitent Internet.

## Sources et limites

- Limites régionales : GeoJSON des 14 régions (ADM1), diffusé dans le dépôt public `bineta66/barakagive`, fichier `frontend/src/data/senegal-regions.geojson`. Les géométries sont adaptées à une carte nationale, pas à un usage cadastral.
- Structures sanitaires complémentaires : OpenStreetMap / Overpass. Les données sont contributives et peuvent contenir des omissions, doublons ou coordonnées imprécises.
- Référence sanitaire officielle : [portail eSanté / CSSDOS](https://www.esante.sn/) et [liste du ministère](https://sante.gouv.sn/publications/liste-des-structures-de-sanitaires-au-s%C3%A9n%C3%A9gal).

Les points OpenStreetMap ne constituent pas un inventaire officiel exhaustif du ministère. Pour une planification sanitaire ou une décision opérationnelle, les vérifier auprès de la CSSDOS / du ministère.

## Attribution

L'interface SVG et le détail de Dakar proviennent du fichier initial fourni par le projet. Les géométries régionales proviennent d'un fichier GeoJSON public référencé ci-dessus. Les objets OpenStreetMap sont soumis à l'ODbL et nécessitent l'attribution OpenStreetMap.
