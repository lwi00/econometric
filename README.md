# Cours d'Économétrie - M2 SIREN

Ce repository contient les travaux pratiques et les données pour le cours d'économétrie de Master 2 SIREN.

## 📋 Table des matières

1. [Prérequis](#prérequis)
2. [Installation](#installation)
3. [Structure du projet](#structure-du-projet)
4. [Guide d'utilisation de Jupyter avec R](#guide-dutilisation-de-jupyter-avec-r)
5. [Premiers pas avec R](#premiers-pas-avec-r)
6. [Travaux pratiques](#travaux-pratiques)
7. [Aide et ressources](#aide-et-ressources)


## 🔧 Prérequis

Avant de commencer, vous aurez besoin d'installer les logiciels suivants sur votre ordinateur :

### 1. Python et Jupyter
- **Python** : Téléchargez depuis [python.org](https://www.python.org/downloads/)
- **Jupyter Notebook** : Sera installé avec les instructions ci-dessous

### 2. R
- **R** : Téléchargez depuis [r-project.org](https://www.r-project.org/)

### 3. VSCode (Recommandé)
- **Visual Studio Code** : Téléchargez depuis [code.visualstudio.com](https://code.visualstudio.com/)
- **Extensions utiles** : Python, R, Jupyter (seront installées plus tard)

## 💻 Installation

### Étape 1 : Installer VSCode et ses extensions

1. **Téléchargez et installez VSCode** depuis [code.visualstudio.com](https://code.visualstudio.com/)
2. **Ouvrez VSCode** et installez les extensions suivantes :
   - Cliquez sur l'icône Extensions (carré avec 4 petits carrés) dans la barre latérale gauche
   - Recherchez et installez :
     - **Python** (Microsoft)
     - **R** (REditorSupport)
     - **Jupyter** (Microsoft)
     - **R Debugger** (RDebugger)

### Étape 2 : Installer les dépendances Python
```bash
# Installez Jupyter et les packages nécessaires
pip install jupyter
pip install IRkernel
```

### Étape 3 : Configurer R pour Jupyter
Ouvrez R (tapez R depuis le terminal) et exécutez les commandes suivantes :
```r
# Installer les packages R nécessaires
install.packages(c("IRkernel", "data.table", "ggplot2", "dplyr"))

# Configurer le kernel R pour Jupyter
IRkernel::installspec()
```

### Étape 4 : Vérifier l'installation
```bash
# Démarrez Jupyter Notebook
jupyter notebook
```
Une page web devrait s'ouvrir automatiquement. Si vous voyez "R" dans la liste des kernels disponibles, l'installation est réussie !

## 📁 Structure du projet

```
econometric/
├── README.md           # Ce fichier
├── requirements.txt    # Dépendances Python
├── day1/              # Travaux pratiques jour 1
│   └── first_lab.ipynb
├── day2/              # Travaux pratiques jour 2
│   ├── lab1.ipynb
│   └── 2018-citibike-tripdata/  # Données CitiBike 2018
│       ├── 1_January/
│       ├── 2_February/
│       └── ...
```


## 📚 Guide d'utilisation de Jupyter avec R

### Qu'est-ce que Jupyter Notebook ?
Jupyter Notebook est un environnement interactif qui permet de :
- Écrire et exécuter du code R (ou Python)
- Visualiser immédiatement les résultats
- Mélanger code, texte explicatif et graphiques
- Sauvegarder tout le travail dans un seul fichier

### Comment démarrer ?

1. **Ouvrir un terminal/invite de commandes**
2. **Naviguer vers le dossier du projet** :
   ```bash
   cd /chemin/vers/econometric
   ```
3. **Lancer Jupyter** :
   ```bash
   jupyter notebook
   ```
4. **Votre navigateur s'ouvre automatiquement** avec l'interface Jupyter

### Interface Jupyter - Les bases

#### Créer un nouveau notebook R :
1. Cliquez sur "New" (Nouveau)
2. Sélectionnez "R" dans la liste

#### Types de cellules :
- **Code** : Pour écrire du code R
- **Markdown** : Pour écrire du texte explicatif
- **Raw** : Texte brut (rarement utilisé)
