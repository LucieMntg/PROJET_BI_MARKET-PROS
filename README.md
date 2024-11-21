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



## Organisation du répertoire
    
    ├───.streamlit                                                <- Code renfermant le thème graphique de l'application Streamlit
    │
    ├───Dataset                                                   <- Dataset avec les données brutes non transformées
    │
    ├───Images                                                    <- Visuels utilisés dans l'application Streamlit
    │
    ├───Modèles                                                   <- Modèles entraînés et prédictions
    │
    ├───Notebooks                                                 <- Jupyter notebooks contenant le code de préprocessing des données et de modélisation
    │       CODE_PROJET_CO2_EXPLORATION_DONNEES.ipynb             <- Exploration des données et visualisation
    │       CODE_PROJET_CO2_PREPROCESSING_MODELISATION.ipynb      <- Feature engineering, pré-processing et modélisation
    │
    ├───Rapport                                                   <- Rapport détaillé du projet au format PDF 
    │
    │   .gitignore                                                <- Fichier Gitignore pour ignorer certains fichiers/dossiers
    │   LICENSE.txt                                               <- Licence du projet
    │   README.md                                                 <- Fichier README avec présentation du projet et lien de l'application streamlit
    │   requirements.txt                                          <- Liste des dépendances Python nécessaires pour reproduire l'environnement
    │   streamlit_project_code_final.py                           <- Code source pour l'application Streamlit








