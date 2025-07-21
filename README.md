Projet Emission de CO2 par les véhicules
 
 
Contexte:
 
Ce projet a été effectué dans le cadre de la formation de Data Scientist dispensée par l'organisme de formation Datascientest et l'école des Mines de Paris (promotion Bootcamp de Mars 2024)
 
 
Objectif :
 
Construire des modèles d'estimations d'émissions de CO2 en roulage afin de prédire à l'avance les émissions de nouveaux types de véhicules (nouvelles séries de voitures par exemple).
 
 
Jeux de données:
 
Deux jeux de données étaient à disposition : 
 * Data.gouv.fr : regroupant l’ensemble des caractéristiques techniques des véhicules commercialisés en France en 2013, ainsi que les consommations de carburant, les émissions de CO2 et les émissions de polluants dans l’air
 * Agence Européenne de l'environnement : regroupant les émissions de CO2 de tous les véhicules commercialisés chaque année en Europe + UK 
  
Pour le projet, nous avons choisi d'analyser la deuxième base de données (https://www.eea.europa.eu/data-and-maps/data/co2-cars-emission-20), en utilisant les données de l'année 2022 (dernières données disponibles), afin de prendre en compte les données les plus récentes avec un nombre de véhicules très important (~10 000 000 de véhicules)
Les véhicules électriques n'émettant pas de CO2 en roulage ,nous avons choisi de ne pas les prendre en compte.

Les codes de data cleaning ainsi que les modèles sont disponibles dans le dossier notebooks (Preprocessing, Modélisation_ML, Modélisation_DL). Pour des raisons de stockage, la base de données n'est pas présente dans le github mais disponible sur le lien ci-dessus (le nom du fichier devra ainsi être modifier en conséquence lors de l'execution du notebook Preprocessing poour l'importation de la data).
 
 
Conclusion et perspectives:
 
Nous avons testé plusieurs modèles de Machine Learning et de Deep Learning et montré qu'il était possible d'obtenir de très bonnes prédictions  (R² > 99%).
Les modèles XGBoost, RandomForest , Arbres de Décision et certains modèles de Deeplearning ont donné les meilleurs résultats.
 
L'étude s'est focalisé sur les seules émissions des véhicules thermiques ou hybrides. Il s'avère que pour réduire sensiblement les émissions de CO2, la proportion de véhicules électriques va s'accroitre régulièrement jusqu'à représenter 100% des véhicules neufs vendus (avec les véhicules à "hydrogène") après 2035.
Une perspective intéressante serait de collecter des données plus globales, prenant en compte tout le cycle de vie du véhicule , afin d'identifier les émissions de CO2 à chaque étape (fabrication, transport, génération de l'électricité, recyclage) et fournir un modèle des émissions de CO2 plus représentatif des émissions réelles.
 
 
Acteurs du projet:
Sarah Hemmel
Saoussen Chaouch
Yamadou Tounkara
Jean-marc Allègre
Elliot Douieb(mentor Datascientest du projet)


--------

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>
