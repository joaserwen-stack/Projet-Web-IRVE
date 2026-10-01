# Écosystème IRVE - Interface Web & Cartographique

## Présentation
Cette application web constitue la troisième et dernière phase du projet global d'analyse du réseau français des Infrastructures de Recharge pour Véhicules Électriques (IRVE). 
Elle offre une interface graphique interactive permettant de visualiser les données géospatiales et d'exploiter les modèles d'Intelligence Artificielle (prédiction et clustering) développés dans les phases précédentes.

## Fonctionnalités Principales
* **Exploration Interactive :** Tableau de bord détaillé des points de charge.
* **Cartographie Web (Leaflet) :** Visualisation spatiale des stations de recharge sur la carte de France.
* **Statistiques Dynamiques :** Analyse et affichage des métriques filtrées par département.
* **Intégration IA (Machine Learning) :** 
  * Appel serveur des scripts Python pour prédire le type d'implantation d'une borne.
  * Prédiction de la puissance nominale via les modèles Scikit-Learn.
  * Regroupement et affichage des clusters de positionnement directement sur la carte.

## Stack Technique
* **Front-end :** HTML5, CSS3, JavaScript, Leaflet (Cartographie), AJAX.
* **Back-end :** PHP, Python (Scripts IA).
* **Base de données :** MySQL.
* **Déploiement :** Docker & Docker-Compose (Architecture de micro-services conteneurisés).

##  Installation & Déploiement (Docker)
L'environnement de l'application est entièrement conteneurisée pour garantir un déploiement simple, rapide et sans conflit de dépendances.

1. Clonez ce dépôt sur votre machine locale :
```bash
git clone https://github.com/joaserwen-stack/Projet-Web-IRVE.git
```

2. Accédez au répertoire du projet :
```bash
cd Projet-Web-IRVE
```

3. Construisez et lancez les conteneurs en arrière-plan :
```bash
docker-compose up -d
```

4. Accédez à l'application via votre navigateur à l'adresse locale classique (généralement `http://localhost`).
