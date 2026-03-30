# Analyse des performances e-commerce (Python & Power BI)

## Objectif
Ce projet vise à analyser les performances commerciales d’une entreprise e-commerce afin d’évaluer sa rentabilité et sa capacité à atteindre ses objectifs de vente.
L’analyse combine préparation des données avec Python et visualisation avec Power BI pour fournir une vision claire et actionnable des performances.

## Données
Le projet s’appuie sur trois fichiers :
List of Orders : informations sur les commandes (date, client, localisation)
Order Details : détails des ventes (produits, quantités, chiffre d’affaires, profit)
Sales Target : objectifs de ventes par catégorie et par mois

## Méthodologie
🔹 1. Préparation des données (Python)
Nettoyage des données (valeurs manquantes, formats)
Conversion des types (dates, variables numériques)
Fusion des tables via les clés de jointure
Création de variables (mois, année, marge)  
🔹 2. Analyse exploratoire
Calcul des KPI : chiffre d’affaires, profit, marge
Analyse par catégorie
Analyse temporelle (évolution mensuelle)
Identification des anomalies (profits négatifs)
🔹 3. Visualisation (Power BI)
Construction d’un modèle de données relationnel
Création de mesures DAX :
Sales
Profit
Margin %
Target
Achievement %
Développement d’un dashboard interactif

## Dashboard
Le dashboard permet de suivre :
Les KPI globaux (CA, profit, marge)
Les performances par catégorie
L’évolution mensuelle des ventes et du profit
La comparaison ventes réelles vs objectifs
Le taux d’atteinte des objectifs (Achievement %)

## Insights clés
Electronics est la catégorie la plus performante, dépassant largement ses objectifs (128%)
Clothing est en sous-performance, avec seulement 80% des objectifs atteints
Furniture génère du chiffre d’affaires mais présente une faible rentabilité
Plusieurs mois présentent un profit négatif, indiquant des périodes non rentables
La performance globale atteint ~99% des objectifs, avec des disparités importantes entre catégories

## Recommandations
Optimiser la stratégie de pricing et les coûts sur la catégorie Furniture
Analyser les causes de sous-performance de Clothing
Capitaliser sur la catégorie Electronics comme levier de croissance
Investiguer les périodes déficitaires pour réduire les pertes

## Outils utilisés
Python (Pandas)
Power BI

## Conclusion
Ce projet met en évidence l’importance d’une analyse combinant performance réelle et objectifs pour piloter efficacement un business e-commerce.
Il démontre également la valeur d’un dashboard interactif pour faciliter la prise de décision.


