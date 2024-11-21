# Projet de Business Intelligence : MARKET PROS

## Présentation

Ce répertoire contient fichier .pbix de ce projet Power BI ainsi que les datasets utilisés pour réaliser ces rapports.

L'objectif était de concevoir plusieurs rapports pour suivre et analyser les performances globales, commerciales et RH de la société Market Pros. La société en question est un Call Center.



## Objectif du projet 

L'objectif principal était de créer des rapports interactifs dans Power BI pour fournir des insights détaillés sur la performance de l'entreprise. Les rapports permettent de suivre les indicateurs clés de performance (KPI) dans les domaines suivants :

- **Performance globale de l'entreprise** : suivi du nombre total des appels et analyse de la qualité des appels.
- **Performances commerciales** :  suivi des ventes par période, par zone géographique, et par type de service concerné.
- **Ressources humaines (RH)** : analyse des performances relatives aux employés et aux managers.




## Étapes du Projet

Les principales étapes réalisées pour ce projet sont les suivantes :

1. **Importation des sources de données** : 
   - Les données ont été extraites et chargées dans Power Query, à partir de fichiers plats, notamment au format Excel et CSV. 

2. **Nettoyage et transformation des données** : 
   - Power Query a été utilisé pour effectuer les premières étapes de préparation et de transformation des données, comprenant le changement de type des colonnes, des modifications structurelles (ajout, suppression ou renommage de colonnes), la supression des doublons et la gestion des valeurs manquantes, la fusion de tables, la définition de catégories de données (Data Category), ainsi que l’agrégation des informations pour les rendre exploitables dans le modèle Power BI.

3. **Modélisation des données** : 
   - Les données ont été organisées dans un modèle analytique en suivant une modélisation en étoile (star schema), ce qui garantit des performances optimales et une analyse cohérente. Ce modèle comprend une table de faits (contenant les données quantitatives à analyser, telles que les ventes ou le nombre d'appels) et plusieurs tables de dimensions (contenant des informations contextuelles, comme les dates, les produits ou les zones géographiques).
   - Des relations ont été définies entre les tables de faits et les tables de dimensions pour assurer leur intégrité et faciliter les calculs.
   - Une table de calendrier personnalisée a été créée pour prendre en charge les analyses temporelles (comparaisons par année, mois, trimestre).
   - De plus, des mesures explicites ont été développées à l’aide du langage DAX pour calculer des indicateurs clés de performance (KPI) et répondre aux besoins métier.
   - Un des objectifs de cette phase était de retirer la complexité technique souvent présente dans les données sources. Pour cela, un travail de simplification sémantique a été effectué, notamment en renommant proprement les tables et les colonnes dans Power Query afin que les utilisateurs puissent facilement comprendre et exploiter les données. Ce travail a permis de rendre le dataset plus accessible et orienté métier.

4. **Création des rapports Power BI** : 
   - Des rapports interactifs ont été créés pour visualiser et analyser les données de manière dynamique. 
   - Une barre de filtrage est disponible afin de permettre aux utilisateurs de filtrer les données selon l'année, le mois et la zone géographique.

5. **Mise en forme et personnalisation** :
   - Les rapports ont été mis en page selon la charte graphique de l'entreprise.


Ce projet a été mené en novembre 2024.



## Environnement technique

Power BI (connexion à plusieurs sources de données, traitement de la donnée, modélisation en étoile avec Power Query, visualisation dynamique).


## Visualisation du projet

Étant donné que les rapports interactifs ne peuvent pas être visualisés directement sur GitHub, plusieurs extraits sont disponibles dans le dossier 'Extract' de ce répertoire, incluant des captures d'écran des visualisations Power BI ainsi que les rapports au format PDF.



## Organisation du répertoire
    
   ├───Dataset                                      <- Dossier renfermant les sources de données utilisées dans ce projet (fichiers plats au format Excel et CSV)
   │   │   Call Charges.xlsx
   │   │   Call+Center+Data+2021.xlsx
   │   │   Lookup+Tables.xlsx
   │   │
   │   └───csv
   │           Call+Center+Data+2018.csv
   │           Call+Center+Data+2019.csv
   │           Call+Center+Data+2020.csv
   │
   ├───Extract                                     <- Dossier renfermant les rapports au format PDF ('Report') et des captures écrans en mode Report View 
   │       Model_view.png                          <- Vue de la modélisation en étoile (Star Schema) utilisée pour organiser les données
   │       Model_view_filter_example.png           <- Vue d'une page du rapport avec filtre sélectionné
   │       Report.pdf                              <- Rapport complet généré sous format PDF pour un aperçu général du projet
   │       Report_view_template.png                <- Vue de la page 'Template' du rapport, qui sert de modèle graphique pour toutes les pages du rapport (page cachée)
   │
   └───Template                                    <- Dossier contenant les éléments graphiques et visuels utilisés pour la mise en forme du rapport
         Template.png                              <- Visuel de fond pour la page 'Template', qui définit la charte graphique du projet
   │   LICENSE.txt                                 <- Fichier contenant les informations de licence concernant les droits d'utilisation du projet
   │   Projet_call_center.pbix                     <- Fichier Power BI contenant l'ensemble du projet 
   │   README.md                                   <- Fichier Markdown avec une description complète du projet, de son objectif et de sa mise en œuvre









