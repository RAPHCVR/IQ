# IQ01 : Introduction à l'Informatique Quantique (UTC)

![Python](https://img.shields.io/badge/Python-3.10%2B-%233776AB?style=for-the-badge&logo=python)
![Qiskit](https://img.shields.io/badge/Qiskit-0.45%2B-blue?style=for-the-badge&logo=ibm)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter)

Ce dépôt rassemble l'ensemble des travaux réalisés dans le cadre de l'unité de valeur **IQ01 - Introduction à l'Informatique Quantique** à l'**Université de Technologie de Compiègne (UTC)**. Il contient les travaux pratiques (TP) qui explorent les concepts fondamentaux et les algorithmes de l'informatique quantique, ainsi qu'un projet de recherche approfondi sur une application potentielle de cette technologie.

## Table des matières
1. [À propos du projet](#à-propos-du-projet)
2. [Travaux Pratiques (TP)](#travaux-pratiques-tp)
    - [TP2 : Fondamentaux de Qiskit et Portes Quantiques](#tp2--fondamentaux-de-qiskit-et-portes-quantiques)
    - [TP3 : Algorithmes Quantiques - Deutsch-Jozsa et Simon](#tp3--algorithmes-quantiques---deutsch-jozsa-et-simon)
    - [TP4 : Étude de Cas - Le Problème de Monty Hall](#tp4--étude-de-cas---le-problème-de-monty-hall)
3. [Projet de Recherche : Résolution des Équations de Navier-Stokes](#projet-de-recherche--résolution-des-équations-de-navier-stokes-par-linformatique-quantique)
4. [Technologies Utilisées](#technologies-utilisées)
5. [Comment utiliser ce dépôt](#comment-utiliser-ce-dépôt)
6. [Auteurs](#auteurs)

## À propos du projet

L'objectif de ce cours était de fournir une introduction solide aux principes de l'informatique quantique. Les travaux pratiques nous ont permis de nous familiariser avec le framework **Qiskit d'IBM** pour construire et simuler des circuits quantiques. Le projet de recherche nous a donné l'opportunité d'explorer comment ces concepts pourraient être appliqués pour résoudre des problèmes complexes, encore hors de portée des ordinateurs classiques.

## Travaux Pratiques (TP)

Les notebooks Jupyter des TPs contiennent des implémentations de concepts clés en informatique quantique.

### TP2 : Fondamentaux de Qiskit et Portes Quantiques
Ce TP couvre les bases de la manipulation de qubits avec Qiskit.
- **Concepts explorés** :
  - Différence entre bit classique et qubit (superposition, intrication).
  - Implémentation des portes quantiques de base : Hadamard (H), Pauli-X (NOT), CNOT, SWAP.
  - Création d'un **état de Bell**, illustrant le phénomène d'intrication.
  - Simulation du protocole de **téléportation quantique**.
- **Fichiers** : `TP2/tp2-ex1-2-3.ipynb`, `TP2/tp2-ex4.ipynb`

### TP3 : Algorithmes Quantiques - Deutsch-Jozsa et Simon
Ce TP se concentre sur les premiers algorithmes démontrant la supériorité quantique pour des problèmes spécifiques.
- **Concepts explorés** :
  - **Algorithme de Deutsch-Jozsa** : Distinguer une fonction constante d'une fonction équilibrée en une seule évaluation.
  - **Algorithme de Simon** : Trouver la période d'une fonction, un problème précurseur de l'algorithme de Shor.
  - Utilisation du concept d'**oracle** pour encapsuler la fonction à étudier.
- **Fichier** : `TP3/tp3.ipynb`

### TP4 : Étude de Cas - Le Problème de Monty Hall
Ce TP utilise un circuit quantique pour modéliser le célèbre paradoxe probabiliste.
- **Concepts explorés** :
  - Modélisation d'un problème probabiliste avec des qubits.
  - Comparaison entre une simulation classique (Monte-Carlo) et un circuit quantique qui représente les probabilités de gain.
  - Le circuit démontre que la stratégie de changer de porte après la révélation du présentateur offre **2/3 de chances de gagner**, contre 1/3 en gardant son choix initial.
- **Fichier** : `TP4/tp4.ipynb`

## Projet de Recherche : Résolution des Équations de Navier-Stokes par l'Informatique Quantique

Ce projet constitue une exploration théorique de l'application de l'informatique quantique à l'un des problèmes les plus célèbres de la physique et des mathématiques appliquées.

- **Titre complet** : `Résolution des équations de Navier-Stokes par l'informatique quantique`
- **Auteurs** : Raphael Chauvier, Robin Dereux, Raphael Nguyen
- **Document** : [Rapport_Navier_Stokes_Quantique.pdf](<chemin_vers_votre_pdf/Rapport_IQ01.pdf>) (Pensez à renommer et lier le PDF ici)

### Résumé du projet
Les équations de Navier-Stokes, qui décrivent la dynamique des fluides, sont notoirement difficiles à résoudre analytiquement et numériquement en raison de leur non-linéarité. Ce rapport étudie le potentiel des ordinateurs quantiques pour surmonter certaines de ces limitations.

Notre analyse explore :
1.  **Les limites des méthodes classiques** : Nous avons étudié les défis computationnels des méthodes de résolution numérique comme la Méthode des Éléments Finis (FEM).
2.  **L'intégration d'algorithmes quantiques** : Nous avons examiné comment des algorithmes quantiques, notamment le **Quantum Linear Equations (QLE)**, pourraient accélérer la résolution des systèmes d'équations linéaires qui sont au cœur des solveurs FEM.
3.  **Conclusion** : Bien qu'une solution entièrement quantique reste lointaine, notre recherche conclut que des **approches hybrides** (classique-quantique) pourraient offrir une **amélioration de complexité polynomiale** pour des sous-problèmes spécifiques. Cela ouvre des perspectives prometteuses pour la simulation de fluides complexes à l'avenir.

## Technologies Utilisées
- **Langage** : Python 3
- **Framework quantique** : Qiskit (SDK IBM Quantum)
- **Bibliothèques Python** : NumPy, Matplotlib
- **Environnement** : Jupyter Notebook
- **Rédaction du rapport** : LaTeX

## Comment utiliser ce dépôt

Pour explorer les notebooks de ce projet, suivez ces étapes :

1.  **Clonez le dépôt :**
    ```bash
    git clone https://github.com/RAPHCVR/IQ.git
    cd IQ
    ```

2.  **Créez un environnement virtuel (recommandé) :**
    ```bash
    python -m venv venv
    source venv/bin/activate  # Sur Windows: venv\Scripts\activate
    ```

3.  **Installez les dépendances :**
    Créez un fichier `requirements.txt` avec le contenu suivant, puis installez-le.
    ```
    # requirements.txt
    qiskit
    qiskit-ibm-runtime
    qiskit_textbook
    numpy
    matplotlib
    ```
    ```bash
    pip install -r requirements.txt
    ```

4.  **Lancez Jupyter Notebook :**
    ```bash
    jupyter notebook
    ```
    Vous pouvez maintenant naviguer dans les dossiers `TP2`, `TP3`, `TP4` et exécuter les notebooks.

## Auteurs
Ce projet a été réalisé par :
- **Raphael Chauvier** ([@RAPHCVR](https://github.com/RAPHCVR))
- **Robin Dereux**
- **Raphael Nguyen**
