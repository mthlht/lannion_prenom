library(tidyverse)
library(lubridate)


# Objectif de cet exercice : vous allez devoir interroger la base de données prénoms de l'Insee
# Vous pouvez trouver la documentation des données via le lien ci-dessous
# => https://www.insee.fr/fr/statistiques/2540004?sommaire=4767262&q=pr%C3%A9noms

# Inutile de télécharger les données depuis l'Insee, elles sont déjà dans le dossier data/raw

# Le dossier data/raw contient deux fichiers CSV :
#   - un fichier de données nationales nommé "prenom_dep_2020.csv" qui contient
#   les prénoms attribués aux enfants nés en France hors Mayotte entre 1900 et 2020
#   et les effectifs par sexe associés à chaque prénom
#   - un fichier de données départementales nommé "prenom_dep_2020" qui contien
#   les mêmes informations au niveau département de naissance

## Les fichiers contenus dans le dossier data/raw/insee_reg sont réservés au Niveau 2

# L'exercice comporte deux niveaux : un premier sur les données nationales,
# un deuxième sur les données départementales

#-------------------------------------------------------------------------------
#-------------------------------------------------------------------------------
#-------------------------------------------------------------------------------
#-------------------------------------------------------------------------------

# NIVEAU 1 - LES DONNÉES NATIONALES


## QUESTION 1
## Charger les données du fichier "prenom_natio_2020.csv en data frame, dans une
## variable raw_natio
## Astuces : le fichier csv doit se lire avec la fonction read_delim()
## et les séparateurs des colonnes sont des ";"






##------------------------------------------------------------------------------

## QUESTION 2
## Dans une variable raw_natio_2020, filtrez uniquement les prénoms donnés en 2020
## Gardez toutes les lignes sauf celles dont la colonne preusuel indique "_PRENOMS_RARES"
## Transformez la casse des prénoms pour avoir une majuscule à la première lettre
## Astuce : vous aurez besoin des fonction filter() et str_to_title()






##------------------------------------------------------------------------------

## QUESTION 3
## Dans une variable natio_g_2020, filtrez uniquement les dix prénoms les plus
## donnés pour les garçons en 2020
## Astuce : la fonction slice_max() peut vous aider, à vous de regarder comment
## elle fonctionne avec l'aide de la fonction

## ATTENTION indiquez bien les noms de vos paramètres dans la fonction slice_max
## fonction(param=arg, param=arg)





##------------------------------------------------------------------------------

## QUESTION 4
## Dans une variable natio_f_2020, filtrez uniquement les dix prénoms les plus
## donnés pour les filles en 2020






##------------------------------------------------------------------------------

## QUESTION 5
## En une seule fois dans, un même dataframe affecté dans une variable natio_fg_2020,
## filtrez uniquement les dix prénoms les plus donnés pour les filles en 2020 d'une part
## et pour les garçons en 2020 d'autre part
## Astuce : vous aurez besoin de la fonction group_by() puis de la fonction slice_max()






##------------------------------------------------------------------------------

## QUESTION 6
## Dans une variable tidy_natio ne gardez que le prénom le plus donné pour les filles et pour les garçons
## pour chaque année.
## Astuce : vous aurez besoin de repartir depuis votre première variable raw_natio
## Pensez à refaire les opérations de la question 2, notamment pour les écarter
## les "_PRENOMS_RARES"


#-------------------------------------------------------------------------------
#-------------------------------------------------------------------------------
#-------------------------------------------------------------------------------


# NIVEAU 2 - LES DONNÉES DÉPARTEMENTALES

## QUESTION 1
## Charger les données du fichier "prenom_dep_2020.csv en data frame, dans une
## variable raw_dep_repnom





## QUESTION 2
## Charger les données du fichier des fichiers "insee_departement.csv" et "insee_region.csv'
## en data frame, respectivement dans les variables insee_dep et insee_reg
## les deux fichiers sont dans le dossier data/raw/insee_dep_reg
## DANS LE DATA FRAME INSEE_REG ne conservez que la colonne REG et la colonne LIBELLE
## et renommez la colonne LIBELLE en reg_nom
## Astuce : les séparateurs sont des "," pour ces ceux fichiers
## Astuce : pour sélectionner et renommer des colonnes la fonction select() peut vous
## être utile





## QUESTION 3
## Dans une variable tidy_dep_reg, ne gardez que trois colonnes de votre data frame
## des départements (les colonnes DEP, REG et LIBELLE) et en sélectionnonant ces colonnes
## renommez la colonne LIBELLE en dep_nom. Puis faites une jointure du data frame region
## Astuce : la fonction left_join() vous sera utile






## QUESTION 4
## Dans une variable raw_bretagne, faites une jointure entre votre data frame stocké
## dans la variable raw_dep et le data frame stocké dans la variable tidy_dep_reg
## puis filtrez uniquement les lignes de la région Bretagne






## Question 5
## Dans une variable tidy_bretagne, réduisez votre data frame de manière à avoir
## la somme de la variable nombre pour chaque prénom par année et par sexe pour chaque année
## Astuce : vous aurez besoin des fonctions group_by(), summarise() et sum()






##------------------------------------------------------------------------------
##------------------------------------------------------------------------------
##------------------------------------------------------------------------------
##------------------------------------------------------------------------------


## BONUS
## Visualisez les résultats de la question 6 du niveau 1 et de la question 5 du niveau 2
## depuis l'année 2000 jusqu'en 2020
## Astuce : Vous aurez besoin des fonctions ggplot() et geom_bar()
## Astuce : transformez votre colonne année en chaine de caractère peut vous aider avec
## les fonctions mutate as.character()






