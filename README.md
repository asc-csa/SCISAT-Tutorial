<!-- Placeholder for tutorial image (required) -->
<p align="center">
   <img src="https://www.asc-csa.gc.ca/images/recherche/hi-res/SatBG2_hr.jpg" alt="Image du SCISAT | Image of SCISAT" height=300>
   <br> Crédit d'image | Image credit: <a href="https://www.asc-csa.gc.ca/eng/satellites/scisat/">ASC-CSA</a>
</p>

<!-- Common badge header (required)
For changing the links, update the first four src=links and replace the section in the link of {{your-tutorial-name}} with the name of your tutorial seen in the url of the GitHub repository. -->
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

<!-- This should not need to be updated unless you change the "id" section of the title section (required) -->

---

<h3 align="center">
  <a href="#titre-du-projet">Français</a> |
  <a href="#project-title">English (follows)</a>
</h3>

---

<!-- ============ FRANÇAIS ============
An engaging title for the project (required)-->
<a id="titre-du-projet"></a>
# SCISAT - Tutoriel

<!-- A short summary phrase for the project (required)-->
> **Description brève :**
> Ce tutoriel démontre le processus d'accès aux données SCISAT, de les préparer pour l'utilisation, et de montrer quelques analyses et visualisations de données de base.


## À propos

<!-- Summary of the use of the tutorial (required)-->
**SCISAT - Tutoriel** est un tutoriel Jupyter Notebook qui guide les utilisateurs à travers l'accès, la préparation et l'analyse des données SCISAT. Il couvre :

- Accès aux données SCISAT via le portail de données ouvertes de l'ASC
- Préparation et traitement des données de concentration de gaz atmosphériques
- Analyses de base et visualisations avec emphasis sur l'ozone
- Application de filtres simples pour une exploration approfondie

Lancé pour la première fois en 2003, SCISAT est un satellite qui aide les scientifiques du Canada et du monde entier à étudier et à apprendre les concentrations de gaz atmosphériques, en particulier l'appauvrissement de la couche d'ozone. Toujours actif aujourd'hui, SCISAT recueille des données sur plus de 60 gaz atmosphériques différents.

*Ce tutoriel est fourni à des fins pédagogiques et expérimentales.*



<!-- Describe any requirements for the deployment (required) -->
## Prérequis

- Python 3.8
- Jupyter Notebook ou Jupyter Lab
- Connexion Internet (pour le téléchargement des données SCISAT)
- Bibliothèques scientifiques Python (NumPy, Matplotlib, Pandas, etc.)



## Démarrage rapide
<!-- The process for setting up your tutorial. Use one of the following:
pip freeze > requirements.txt

The method above will likely require some level of cleaning to create a good requirements.txt. Alternatively, you can try pip-chill to help create a better cleaner requirements.txt.

pip install pip-chill
pip-chill --no-chill -v > requirements.txt

Or if you prefer to specify a conda environment:
conda env export --no-builds | grep -v "^prefix: " > environment.yml
 (required) -->
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
   # ou
   conda install -c conda-forge --file requirements.txt
   ```
4. 🚀 **Lancer le tutoriel**
   ```bash
   jupyter notebook scisat_tutorial.ipynb
   ```

> **Remarque :** Les graphiques ne s'affichent pas dans GitHub, et vous devrez configurer le projet localement pour les visualiser.



<!-- It can be helpflul to describe the different tools users will learn from your tutorial (optional) -->
## Fonctionnalités

- **Accès aux données :** Télécharger et prétraiter les données SCISAT depuis le portail de données ouvertes
- **Analyse :** Réaliser des analyses de données de base et des visualisations de gaz atmosphériques
- **Filtrage :** Appliquer des filtres simples pour une exploration approfondie
- **Ozone :** Focus spécial sur l'analyse des données de concentration d'ozone



## Modèle de prévision de la concentration d'ozone de SCISAT

En complément à ce tutoriel, vous pouvez trouver une implémentation simple d'un modèle de réseau neuronal prédictif qui utilise les données SCISAT. Le fichier `scisat_mlp.ipynb` présente un guide, étape par étape, de la création et de l'analyse initiale du modèle.

> **Avertissement :** Les prédictions et les résultats statistiques contenus dans ce tutoriel n'ont pas fait l'objet d'un examen scientifique par les pairs et ne doivent pas être utilisés à l'appui d'une analyse ou d'une publication scientifique.

Bien que ce tutoriel utilise des données sur l'ozone, il existe une grande sélection d'ensembles de données sur différents gaz disponibles [ici](https://donnees-data.asc-csa.gc.ca/en/dataset/02969436-8c0b-4e6e-ad40-781cdb43cf24).



<!-- The standard license required for ASC-CSA tutorials (required) -->
## Licence

Ce projet est sous une licence MIT modifiée – voir le fichier [LICENSE](https://github.com/asc-csa/SCISAT-Tutorial/blob/main/LICENSE.txt) pour plus de détails.


<!-- This should not need to be updated unless you change the "id" section of the title section (required) -->

---

<h3 align="center">
  <a href="#project-title">English </a> |
  <a href="#titre-du-projet">Français (précède)</a>
</h3>

---

<!-- ============ English ============
An engaging title for the project (required)-->
<a id="project-title"></a>
# SCISAT Tutorial

<!-- A short summary phrase for the project (required)-->
> **Brief description:**
> This tutorial demonstrates the process of accessing SCISAT data, preparing it for use, and showing basic data analysis and visualization.

<!-- Summary of the use of the tutorial (required)-->
## About

**SCISAT Tutorial** is a Jupyter Notebook tutorial that guides users through accessing, preparing, and analyzing SCISAT data. It covers:

- Accessing SCISAT data via CSA's Open Data Portal
- Preparing and processing atmospheric gas concentration data
- Basic analysis and visualization with emphasis on ozone
- Applying simple filters for further exploration

First launched in 2003, SCISAT is a satellite that helps scientists in Canada and across the globe study and learn about the concentrations of atmospheric gases, with an emphasis on the depletion of the ozone layer. Still active today, SCISAT collects data on over 60 different atmospheric gases.

*This tutorial is provided for educational and experimental purposes.*



<!-- Describe any requirements for the deployment (required) -->
## Prerequisites

- Python 3.8
- Jupyter Notebook or Jupyter Lab
- Internet connection (for SCISAT data download)
- Scientific Python libraries (NumPy, Matplotlib, Pandas, etc.)



## Quick Start
<!-- The process for setting up your tutorial. Use one of the following:
pip freeze > requirements.txt

The method above will likely require some level of cleaning to create a good requirements.txt. Alternatively, you can try pip-chill to help create a better cleaner requirements.txt.

pip install pip-chill
pip-chill --no-chill -v > requirements.txt

Or if you prefer to specify a conda environment:
conda env export --no-builds | grep -v "^prefix: " > environment.yml
 (required) -->

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
   # or
   conda install -c conda-forge --file requirements.txt
   ```
4. 🚀 **Run the tutorial**
   ```bash
   jupyter notebook scisat_tutorial.ipynb
   ```

> **Note:** Plots do not display in GitHub; you will need to set up the project locally to view visualizations.



<!-- It can be helpflul to describe the different tools users will learn from your tutorial (optional) -->
## Features

- **Data Access:** Download and preprocess SCISAT data from the Open Data Portal
- **Analysis:** Perform basic data analysis and visualization of atmospheric gases
- **Filtering:** Apply simple filters for further exploration
- **Ozone Focus:** Special emphasis on ozone concentration data analysis



## SCISAT Ozone Concentration Prediction Model

As an addition to this tutorial, you can find a simple implementation of a predictive neural network model that uses SCISAT data. The notebook found in `scisat_mlp.ipynb` contains a step by step guide of the creation and initial analysis of the model.

> **Disclaimer:** The predictions and statistical results contained in this tutorial have not been scientifically peer-reviewed and should not be used to support any scientific analysis or publication.

While this tutorial uses ozone data, there is a large selection of datasets of different gases available [here](https://donnees-data.asc-csa.gc.ca/en/dataset/02969436-8c0b-4e6e-ad40-781cdb43cf24).

<!-- The standard license required for ASC-CSA tutorials (required) -->
## License

This project is licensed under a modified MIT license - see the [LICENSE](https://github.com/asc-csa/SCISAT-Tutorial/blob/main/LICENSE.txt) file for details.
