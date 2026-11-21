# 📈 Optimisation de la Performance d'un E-commerce

## 🎯 Contexte

Un site e-commerce réalise **432 K de chiffre d'affaires** sur 12 mois (avril 2018 à mars 2019, 500 commandes), réparti sur trois catégories de produits :

* 👕 Clothing
* 💻 Electronics
* 🛋️ Furniture

La marge globale s'établit à **5,5 %** (24 K de profit), mais elle masque une performance très instable : l'entreprise a perdu de l'argent pendant six mois consécutifs.

*Les montants sont exprimés dans l'unité monétaire du jeu de données.*

---

## ❓ Problématique

> Comment stabiliser la rentabilité d'une activité qui alterne pertes et profits, et quels leviers activer en priorité ?

---

## 🔍 Analyse

### Performance économique globale

| Indicateur          | Valeur |
| ------------------- | -----: |
| Chiffre d'affaires  | 432 K  |
| Profit              | 24 K   |
| Marge globale       | 5,5 %  |
| Mois déficitaires   | 6 / 12 |

### Analyse temporelle : deux semestres opposés

| Période                  | CA mensuel moyen | Commandes / mois | Profit cumulé |
| ------------------------ | ---------------: | ---------------: | ------------: |
| Avril → septembre 2018   |             26 K |               33 |      −21,8 K  |
| Octobre 2018 → mars 2019 |             46 K |               51 |      +45,7 K  |

* Les **six premiers mois sont tous déficitaires** (marge mensuelle de −7 % à −21 %), puis les six suivants sont tous bénéficiaires (+10 % à +24 %).
* Pendant la période déficitaire, **les trois catégories perdent de l'argent en même temps** et le volume de commandes est inférieur d'un tiers.

### Analyse par catégorie et sous-catégorie

| Catégorie   | CA    | Profit | Marge | Objectif de ventes atteint |
| ----------- | ----: | -----: | ----: | -------------------------: |
| Clothing    | 139 K | 11,2 K | 8,0 % |                       80 % |
| Electronics | 165 K | 10,5 K | 6,3 % |                      128 % |
| Furniture   | 127 K |  2,3 K | 1,8 % |                       96 % |

Le niveau catégorie ne suffit pas : les écarts se jouent **au niveau des sous-catégories**.

* **Tables** (−4,0 K) et **Electronic Games** (−1,2 K) sont les deux seules sous-catégories déficitaires : elles détruisent 5,2 K de profit, l'équivalent de 22 % du profit total.
* **Bookcases**, pourtant dans Furniture, est la 2e sous-catégorie la plus rentable (+4,9 K) : réduire Furniture dans son ensemble supprimerait aussi ce contributeur.
* **Saree** génère 53,5 K de CA avec une marge de 0,7 % : la catégorie Clothing, rentable en moyenne, porte un enjeu de pricing important.

### Insight principal

> La sous-performance ne vient pas d'une catégorie en particulier : elle est concentrée sur une période (avril à septembre 2018) où la demande est plus faible et où toutes les catégories sont déficitaires. Le mix produit est un levier secondaire, à traiter au niveau des sous-catégories.

---

## 💡 Recommandations

### 1. Piloter la performance mensuellement

* Suivre chaque mois le profit, la marge et le volume de commandes par catégorie
* Déclencher une alerte dès qu'un mois passe sous le seuil de rentabilité

### 2. Soutenir la demande pendant les périodes creuses

* Concentrer les actions commerciales sur les mois à faible volume
* Analyser les causes de la faiblesse d'avril à septembre (saisonnalité, démarrage d'activité, remises) avant d'engager des moyens

### 3. Traiter les sous-catégories déficitaires

* Revoir le prix, les coûts ou le maintien au catalogue de **Tables** et **Electronic Games**
* Conserver et mettre en avant **Bookcases**

### 4. Ajuster le pricing des produits à fort volume et faible marge

* Priorité à **Saree** : un gain de quelques points de marge sur 53,5 K de CA a un effet direct sur le profit global

---

## 🚀 Plan d'Action

### 🟦 Court Terme — Stabilisation

* Mise en place du suivi mensuel du profit par catégorie et sous-catégorie
* Revue du pricing de Tables, Electronic Games et Saree
* Actions commerciales ciblées sur les périodes creuses

**Objectif :** réduire le nombre de mois déficitaires.

### 🟩 Moyen Terme — Optimisation

* Étude de la saisonnalité sur un historique plus long
* Analyse du comportement client
* Ajustement du catalogue au niveau des sous-catégories

**Objectif :** améliorer durablement la rentabilité.

---

## 📊 Indicateurs de Suivi (KPIs)

* Nombre de mois déficitaires
* Profit mensuel minimum
* Marge par sous-catégorie
* Atteinte des objectifs de ventes par catégorie
* Volume de commandes mensuel

---

## 🛠️ Outils

* **Python (Pandas)** : nettoyage, jointure des tables commandes / détails et calcul des indicateurs par catégorie, sous-catégorie et mois
* **Power BI** : tableau de bord de suivi de la performance

---

## ✅ Conclusion

La priorité est de **stabiliser la performance** en évitant de nouvelles séries de mois déficitaires, grâce à un pilotage mensuel et à des actions ciblées sur les périodes creuses. Les corrections de mix et de pricing se font ensuite **au niveau des sous-catégories** (Tables, Electronic Games, Saree) plutôt que par catégorie entière.
