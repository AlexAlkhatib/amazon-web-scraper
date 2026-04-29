# ⛏️ Amazon Web Scraper

Ce projet consiste à développer un **web scraper en Python** permettant d’extraire automatiquement des informations de produits depuis Amazon et de suivre leur évolution dans le temps.

Il illustre l’automatisation de la collecte de données web ainsi que leur stockage et leur exploitation.


## 📁 Structure du Projet

```bash
📦 amazon-web-scraper
 ┣ 📄 Amazon Web Scraper.ipynb
 ┣ 📄 amazon_data.csv (généré)
 ┗ 📄 README.md
```


## 🛠️ Technologies Utilisées

* **Python**
* **BeautifulSoup** (web scraping)
* **Requests** (requêtes HTTP)
* **Pandas** (manipulation des données)
* **Datetime** (suivi temporel)
* **Jupyter Notebook**


## 🎯 Objectifs du Projet

✔️ Extraire des données produits depuis une page Amazon
✔️ Nettoyer et structurer les données récupérées
✔️ Stocker les données dans un fichier CSV
✔️ Suivre l’évolution des prix dans le temps
✔️ Automatiser la collecte de données


## 🔍 Données Collectées

Le scraper permet de récupérer :

* Nom du produit
* Prix
* Date de collecte


## ⚙️ Fonctionnement

1. Envoi d’une requête HTTP vers la page produit
2. Parsing du HTML avec **BeautifulSoup**
3. Extraction des informations (titre, prix…)
4. Nettoyage des données
5. Sauvegarde dans un fichier CSV
6. Possibilité de répéter l’opération pour suivre l’évolution des prix


## 📊 Exemple de Code

```python
import requests
from bs4 import BeautifulSoup

url = "https://www.amazon.com/..."
headers = {"User-Agent": "your-user-agent"}

page = requests.get(url, headers=headers)
soup = BeautifulSoup(page.content, "html.parser")
```


## ▶️ Comment Exécuter le Projet

1. Installer les dépendances :

```bash
pip install requests beautifulsoup4 pandas
```

2. Lancer le notebook :

```bash
jupyter notebook
```

3. Ouvrir :

```bash
Amazon Web Scraper.ipynb
```


## ⚠️ Remarque Importante

Le scraping d’Amazon est soumis à des restrictions :

* Utiliser un **User-Agent** valide
* Respecter les conditions d’utilisation du site
* Éviter les requêtes trop fréquentes


## 📈 Améliorations Possibles

* Automatisation avec tâches planifiées (cron)
* Ajout d’alertes de prix
* Stockage en base de données
* Dashboard de suivi des prix
* Gestion multi-produits


## 💡 Compétences Démontrées

✔️ Web Scraping
✔️ Manipulation HTML / DOM
✔️ Automatisation en Python
✔️ Nettoyage et stockage de données
✔️ Suivi de données dans le temps


## 👤 Auteur

**Alex Alkhatib**
Ingénieur en Intelligence Artificielle — Passionné par la Data et l’automatisation.


## 📄 Licence

MIT License — Copyright (c) 2026 Alex Alkhatib
