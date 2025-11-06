# Écosystème statistiques & connaissances – Jeunes (11–25 ans) en Seine-Saint-Denis (93)

## 0. Périmètre & questions
- **Population cible** : jeunes 11–25 ans, Seine-Saint-Denis (93)
- **Questions clés** :
  1. Quelle densité d’offre (psychologues/psychiatres, CMP, MDA) et où ?
  2. Quel recours aux dispositifs remboursés (Mon Soutien Psy, Santé Psy Étudiant) ?
  3. Quels signaux populationnels (prévalence symptômes anxio-dépressifs, idées suicidaires) ?
  4. Quelles inégalités territoriales/sociales (par commune/quartier) ?

## 1. Sources de données (data brutes)
| Nom | URL | Licence | Format | Période | Description |
|-----|-----|---------|--------|---------|-------------|
| INSEE – Dossier complet 93 | https://www.insee.fr/fr/statistiques/2011101?geo=DEP-93 | ODbL | CSV | 2010–2025 | Indicateurs démographiques |
| CartoSanté / Atlasanté | https://cartosante.atlasante.fr/ | LO | Web | séries | Offre/consommation de soins |
| Démographie des psychologues – IDF (ADELI/RPPS) | PAPS IDF | — | PDF | 2014–2024 | Densité de psychologues |
| Santé Psy Étudiant – séances | https://www.data.gouv.fr/datasets/liste-des-seances-de-psychologie-realisees-sante-psy-etudiant-1/ | LO v2 | CSV | 2021–2024 | Nombre de séances |
| Mon Soutien Psy – infos officielles | https://www.service-public.fr/particuliers/actualites/A17461 | — | HTML | 2025 | Dispositif de droit commun |
| Maisons des Adolescents – IDF | https://anmda.fr/fr/annuaire-mda | — | HTML | — | Annuaire des MDA du 93 |
| ARS IDF – Offre/CMP | https://www.iledefrance.ars.sante.fr/sante-mentale-des-premiers-recours-aux-soins-specialises | — | HTML | 2024–2025 | CMP enfants/adolescents |
| DREES – État des lieux santé mentale | https://drees.solidarites-sante.gouv.fr/publications-communique-de-presse/etudes-et-resultats/250604_ER_sante-mentale-etat-des-lieux | — | HTML | 2025 | Tendances nationales |

## 2. Modèle de tables (schémas)
- **pop_commune** : code_insee, annee, pop_totale, part_0_24  
- **pro_psy** : id, profession, statut, commune, annee  
- **structures** : id, type, nom, commune, lat, lon  
- **dispositifs** : id, nom, annee, nb_seances, territoire  

## 3. Structures visuelles
- Carte choroplèthe : densité psy / 10 000 jeunes + points MDA/CMP  
- Barres comparatives : communes top/bottom densité psy  
- Série temporelle : séances Santé Psy Étudiant par mois  
- Treemap : répartition statuts (libéral/salarié)

## 4. Représentations (viz → question)
- **Line chart** → évolution du recours ?  
- **Bar chart** → communes jeunes/faible offre ?  
- **Map** → déserts psy ?  
- **Scatter** → corrélation offre/besoins ?

## 5. Interactions
Filtres (âge, commune), zoom carte, légende cliquable, survol info-bulle.

## 6. Pipeline
Ingestion CSV → Nettoyage → Jointure → Indicateurs → Viz (D3/Observable) → Publication (GitHub Pages).

## 7. Gouvernance
Lister licences, tracer transformations, définir fréquence MAJ.

## 8. Liens utiles
- D3 Gallery : https://observablehq.com/@d3/gallery
- Markdown GitHub : https://docs.github.com/fr/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax
