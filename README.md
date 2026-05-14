# Projet Machine Learning — Churn Télécom & Segmentation E-commerce

Ce dépôt contient deux projets de Machine Learning réalisés dans le cadre d’un travail académique :

1. **Réduction du churn télécom**
2. **Segmentation clients e-commerce**

L’objectif principal est d’analyser des données clients, de construire des modèles ou segmentations pertinents, puis de proposer des recommandations business exploitables.

---

## Auteur

**Aymen Benbouhia**  
Université Mundiapolis  
Module : Machine Learning / Data Mining  

---

## Contenu du dépôt

```text
Projet ML Telecom/
│
├── README.md
│
├── projet_Churn_telecom.ipynb
├── test.ipynb
├── sujet2_segmentation_ecommerce_notebook.ipynb
│
├── WA_Fn-UseC_-Telco-Customer-Churn.csv
├── Mall_Customers.csv
│
├── presentation_resultats_churn_telecom.pptx
└── presentation_sujet2_segmentation_ecommerce.pptx
```

---

## Projet 1 : Réduction du churn télécom

### Objectif

Le premier projet consiste à analyser le churn des clients d’un opérateur télécom.

Le churn correspond aux clients qui quittent l’entreprise ou résilient leur abonnement.

L’objectif est de :

- Comprendre les facteurs liés au churn
- Identifier les clients à risque
- Comparer plusieurs modèles de classification
- Proposer des actions de fidélisation ciblées

### Dataset utilisé

Le fichier utilisé est :

```text
WA_Fn-UseC_-Telco-Customer-Churn.csv
```

Il contient des informations sur les clients télécom :

- Ancienneté du client
- Type de contrat
- Services souscrits
- Méthode de paiement
- Montant mensuel
- Statut de churn

### Résultats principaux

Les résultats montrent que le churn est un problème important dans le dataset.

Quelques résultats importants :

- 7 043 clients analysés
- Taux de churn : environ 26,5 %
- Meilleur modèle : régression logistique
- ROC-AUC du meilleur modèle : environ 0,84
- Recall du meilleur modèle : environ 78,3 %

### Interprétation

Les clients les plus à risque sont généralement :

- Les clients avec un contrat mensuel
- Les nouveaux clients avec une faible ancienneté
- Les clients avec des mensualités élevées
- Les clients utilisant le paiement électronique

### Recommandations métier

Pour réduire le churn, il est recommandé de :

- Cibler les nouveaux clients dès les premiers mois
- Encourager les contrats de longue durée
- Surveiller les clients avec des mensualités élevées
- Mettre en place des campagnes de rétention
- Utiliser un score de churn pour prioriser les actions CRM

---

## Projet 2 : Segmentation clients e-commerce

### Objectif

Le deuxième projet consiste à segmenter les clients d’un centre commercial ou d’une plateforme e-commerce.

L’objectif est de :

- Comprendre les comportements d’achat
- Regrouper les clients selon leurs similitudes
- Identifier des profils clients
- Proposer des actions marketing adaptées à chaque segment

### Dataset utilisé

Le fichier utilisé est :

```text
Mall_Customers.csv
```

Il contient des informations sur les clients :

- Genre
- Âge
- Revenu annuel
- Spending Score

### Méthode utilisée

La méthode principale utilisée est :

```text
K-Means Clustering
```

Le nombre optimal de clusters choisi est :

```text
k = 5
```

### Segments obtenus

La segmentation a permis d’identifier 5 groupes de clients :

| Cluster | Profil |
|---|---|
| C0 | Budget prudent |
| C1 | Jeunes dynamiques |
| C2 | Premium engagés |
| C3 | Aisés peu actifs |
| C4 | Matures équilibrés |

### Recommandations marketing

Pour chaque segment, des actions marketing peuvent être proposées :

- **C2 — Premium engagés** : programme VIP, ventes privées, offres premium
- **C3 — Aisés peu actifs** : campagnes de réactivation, bundles personnalisés
- **C1 — Jeunes dynamiques** : offres tendance, promotions limitées, gamification
- **C4 — Matures équilibrés** : communication rassurante, offres packagées
- **C0 — Budget prudent** : coupons, réductions, promotions prix

---

## Technologies utilisées

Les outils et bibliothèques utilisés dans ce projet sont :

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Git
- GitHub

---

## Étapes générales du projet

Les deux projets suivent une démarche similaire :

1. Chargement des données
2. Exploration des données
3. Nettoyage et préparation
4. Visualisation
5. Modélisation ou segmentation
6. Évaluation des résultats
7. Interprétation métier
8. Recommandations

---

## Comment exécuter le projet

### 1. Cloner le dépôt

```bash
git clone https://github.com/AymnBen/Mini_Projet_ML.git
```

### 2. Entrer dans le dossier

```bash
cd NOM_DU_REPO
```

### 3. Installer les bibliothèques nécessaires

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

### 4. Lancer Jupyter Notebook

```bash
jupyter notebook
```

Ensuite, ouvrir les fichiers `.ipynb`.

---

## Présentations

Le dépôt contient aussi deux présentations PowerPoint :

- `presentation_resultats_churn_telecom.pptx`
- `presentation_sujet2_segmentation_ecommerce.pptx`

Ces présentations résument les résultats, les visualisations et les recommandations business.

---

## Conclusion

Ce projet permet de mettre en pratique plusieurs compétences importantes en Machine Learning et Data Mining :

- Analyse exploratoire des données
- Préparation des données
- Classification supervisée
- Segmentation non supervisée
- Évaluation de modèles
- Interprétation des résultats
- Proposition de recommandations métier

Le projet montre comment les données peuvent aider une entreprise à mieux comprendre ses clients, réduire le churn et personnaliser ses actions marketing.
