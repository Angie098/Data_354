# Projet Data_354

Ce projet vise à développer un modèle de classification d'images de riz cultivé en Egypte. La classification supervisée s'est faites suivant les classes suivantes : blast, Brown et Healthy. Le modèle est basé sur l'architecture ResNet34 avec l'ajout de mécanisme d'attention.
***
Structure
 
**1.Projet_Data.ipynb:** Notebook contenant le code des transformations faites sur l’ensemble de donnée la construction du modèle et les prédictions fait.
**2.Capture d'écran 2023-12-11:** Capture de la soumission sur Zindi.africa 
**3.submission_results2.csv :** Fichier csv contenant les prédictions du test de notre modèle 
**4.poids.pth:** Fichier pth contenant les poids du modèle entrainé
***
#Modélisation

**Première étape :** Cette étapes a été marquer par l’importation des bibliothèques chargement et traitement des données d’apprentissage.

**Deuxième étape :** Dans cette partie le jeu de donnée d’apprentissage (train.csv)  a été divisé en entrainement et validation, ensuite les transformations d’images ont été définis enfin la creation d’instance des fonction TV_Dataset et DataLoader s’est faite sur les ensembles d’entrainement et validation.

**Troisième étapes :** Définition du module d’attention qui est combiné au modèle ResNet-34 pour effectuer le CNN. Prédiction sur l’ensembles test.csv après les transformations
