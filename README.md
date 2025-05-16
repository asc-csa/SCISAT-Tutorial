
<p align="center">
   <img src="https://www.asc-csa.gc.ca/images/recherche/hi-res/SatBG2_hr.jpg" alt="scisat" height=300> 
   <br> Crédit d'image | Image credit: <a href=https://www.asc-csa.gc.ca/images/recherche/hi-res/SatBG2_hr.jpg>ASC-CSA</a>
</p>

<p align="center">
    <a href="#stars">
        <img alt="Étoiles sur GitHub | GitHub Repo stars" src="https://img.shields.io/github/stars/asc-csa/SCISAT-Tutorial">
    </a>
    <a href="#watchers">
        <img alt="Spectateurs sur Github | GitHub watchers" src="https://img.shields.io/github/watchers/asc-csa/SCISAT-Tutorial">
    </a>
    <a href="https://github.com/asc-csa/SCISAT-Tutorial/commits/main">
        <img alt="Dernier commit sur GitHub | GitHub last commit" src="https://img.shields.io/github/last-commit/asc-csa/SCISAT-Tutorial">
    </a>
    <a href="https://github.com/asc-csa/SCISAT-Tutorial/graphs/contributors">
        <img alt="Contributeurs sur GitHub | GitHub contributors" src="https://img.shields.io/github/contributors/asc-csa/SCISAT-Tutorial">
    </a>
    <a href="https://twitter.com/intent/follow?screen_name=csa_asc">
        <img alt="Suivre sur Twitter | Twitter Follow" src="https://img.shields.io/twitter/follow/csa_asc?style=social">
    </a>
</p>

<h2 align="center">
  <a href="#titre-du-projet">Français</a> |
  <a href="#project-title">English (follows)</a>
</h2>

<a id="titre-du-projet"></a>
# SCISAT-Tutoriel

> **Description brève :**
> Ce tutoriel explique comment accéder aux données du satellite SCISAT, les préparer et les visualiser, en utilisant des mesures liées à l’ozone.

---

## À propos

Lancé pour la première fois en 2003, SCISAT est un satellite qui aide les scientifiques du Canada et du monde entier à étudier et à apprendre les concentrations de gaz atmosphériques, en particulier l'appauvrissement de la couche d'ozone. Toujours actif aujourd'hui, SCISAT recueille des données sur plus de 60 gaz atmosphériques différents. Une grande partie de ces données est disponible sur le portail d'information et de données ouvertes de l'ASC.

Le but de ce tutoriel est de démontrer le processus d'accès à ces données, de les préparer pour l'utilisation, et de montrer quelques analyses et visualisations de données de base en utilisant les données SCISAT. Le tutoriel présente également quelques filtres simples que nous pouvons appliquer aux données pour une exploration plus approfondie.

Bien que ce tutoriel utilise des données sur l'ozone, il existe une grande sélection d'ensembles de données sur différents gaz disponibles [ici](https://donnees-data.asc-csa.gc.ca/en/dataset/02969436-8c0b-4e6e-ad40-781cdb43cf24).


## Démarrage rapide
1. 📦 **Cloner le dépôt**
   ```bash
   git clone https://github.com/asc-csa/SCISAT-Tutorial.git
   cd SCISAT-Tutorial
   ```
2. 🐍 **Créer un environnement**
   ```bash
   # Avec virtualenv
   python -m venv env
   source env/bin/activate

   # Ou avec conda
   conda create -n scisat_env python=3.8
   conda activate scisat_env
   ```
3. 📥 **Installer les dépendances**
   ```bash
   pip install -r requirements.txt
   ```
4. 🚀 **Lancer le tutoriel**
   ```bash
   jupyter notebook scisat_tutorial.ipynb
   ```

> **Remarque :** Si les graphiques ou cartes ne s’affichent pas, redémarrez Jupyter Notebook ou ajoutez `%matplotlib inline` dans la première cellule.

## Fonctionnalités

### Modèle de prévision de la concentration d'ozone de SCISAT

En complément à ce tutoriel, vous pouvez trouver une implémentation simple d'un modèle de réseau neuronal prédictif qui utilise les données SCISAT. Le fichier scisat_mlp.ipynb présente un guide, étape par étape, de la création et de l'analyse initiale du modèle.

Veuillez noter que les prédictions et les résultats statistiques contenus dans ce tutoriel n'ont pas fait l'objet d'un examen scientifique par les pairs et ne doivent pas être utilisés à l'appui d'une analyse ou d'une publication scientifique.

## Licence

Ce projet est  sous une licence MIT modifiée – voir le fichier [LICENSE](https://github.com/asc-csa/SCISAT-Tutorial/blob/main/LICENSE.txt) pour plus de détails.

---

<h2 align="center">
  <a href="#project-title">English </a> |
  <a href="#titre-du-projet">Français (précède)</a>
</h2>


<a id="project-title"></a>
# SCISAT-Tutorial

> **Brief description:**
> This tutorial shows how to access, prepare, and visualize SCISAT satellite data, using ozone-related measurements.

---

## About

First launched in 2003, SCISAT is a satellite that helps scientists in Canada and across the globe study and learn about the concentrations of atmospheric gases, with an emphasis on the depletion of the ozone layer. Still active today, SCISAT collects data on over 60 different atmospheric gases. A large amount of this data is available on CSA's Open Data and Information Portal.

The purpose of this tutorial is to help demonstrate the process of accessing the SCISAT data, preparing it for use, and to show some basic data analysis and visualisation using the SCISAT data. The tutorial also demonstrates some simple filters we can apply to the data for further exploration.

While this tutorial uses ozone data, there is a large selection of datasets of different gases available [here](https://donnees-data.asc-csa.gc.ca/en/dataset/02969436-8c0b-4e6e-ad40-781cdb43cf24).

## Quick Start

1. 📦 **Clone the repo**
   ```bash
   git clone https://github.com/asc-csa/SCISAT-Tutorial.git
   cd SCISAT-Tutorial
   ```
2. 🐍 **Create environment**
   ```bash
   # Using virtualenv
   python -m venv env
   source env/bin/activate

   # Or using conda
   conda create -n scisat_env python=3.8
   conda activate scisat_env
   ```
3. 📥 **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```
4. 🚀 **Run the tutorial**
   ```bash
   jupyter notebook scisat_tutorial.ipynb
   ```

> **Note:** If plots or maps do not display, restart Jupyter Notebook or run `%matplotlib inline` in the first cell.

## Functionality

### SCISAT Ozone Concentration Prediction Model

As an addition to this tutorial, you can find a simple implementation of a predictive neural network model that uses SCISAT data. The notebook found in _scisat_mlp.ipynb_ contains a step by step guide of the creation and initial analysis of the model.

Please be advised that the predictions and statistical results contained in this tutorial have not been scientifically peer-reviewed and should not be used to support any scientific analysis or publication.

## License

This project is licensed under a modified MIT license - see the [LICENSE](https://github.com/asc-csa/SCISAT-Tutorial/blob/main/LICENSE.txt) file for details.

---



