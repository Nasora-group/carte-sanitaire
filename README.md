# Carte sanitaire du Sénégal

Carte SVG interactive adaptée du fichier initial « Carte sanitaire de Dakar ».

## Fonctionnalités

- Vue nationale avec les 14 régions administratives.
- Onglet **Dakar (détail)** conservant la carte initiale des communes et structures.
- Sélection d'une région, panneau d'information, légende par type et affichage adaptatif.
- Limites régionales chargées depuis l'API publique GalsenAPI.
- Points complémentaires recherchés depuis OpenStreetMap via Overpass, au chargement de la page.

## Lancer

Ouvrir `index.html` dans un navigateur connecté à Internet. Les couches nationales dépendent de services externes et ne fonctionneront pas hors ligne.

## Sources et limites

- **Limites régionales** : [GalsenAPI](https://galsenapi.lassanasiby.com/developers/) ; données géographiques issues de HDX/COD-AB, selon la documentation de la source.
- **Structures sanitaires complémentaires** : [OpenStreetMap](https://www.openstreetmap.org/) via Overpass. La couverture est contributive et peut contenir des omissions, doublons ou coordonnées imprécises.
- **Référence sanitaire officielle** : [Portail eSanté / CSSDOS](https://www.esante.sn/). Le portail officiel indique 1 993 structures référencées, dont 1 907 localisées sur sa carte (chiffres affichés lors de la consultation du 23 octobre 2026).

Les points issus d'OpenStreetMap ne doivent pas être considérés comme l'inventaire officiel du ministère. Pour des usages de planification sanitaire, vérifier les données auprès de la CSSDOS/MSHP.

## Attribution

Le style et la carte détaillée de Dakar sont conservés à partir du fichier HTML fourni dans le projet. Les données externes restent soumises aux licences et conditions de leurs sources, notamment l'ODbL pour OpenStreetMap.
