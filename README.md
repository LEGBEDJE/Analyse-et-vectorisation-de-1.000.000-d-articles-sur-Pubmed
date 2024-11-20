# Analyse-et-vectorisation-de-1.000.000-d-articles-sur-Pubmed
Description du projet

Ce projet explore un grand ensemble d'articles scientifiques issus de la base de données PubMed. L'objectif principal est de récupérer, analyser, et regrouper des articles en clusters thématiques en utilisant des techniques de traitement du langage naturel (NLP) et de machine learning non supervisé.
Objectifs principaux

    Récupérer des articles scientifiques depuis l'API PubMed.
    Prétraiter les données textuelles (résumés) pour une analyse NLP efficace.
    Appliquer des techniques avancées :
        Vectorisation des textes avec TF-IDF.
        Réduction de la dimensionnalité avec PCA.
        Clustering des articles avec l'algorithme K-means.
    Visualiser les clusters thématiques des articles.
    Explorer des thématiques potentiellement associées à chaque groupe.

Fonctionnalités

    Extraction automatique des données depuis PubMed via l'API Entrez.
    Nettoyage des données textuelles (normalisation, suppression des stopwords, etc.).
    Calcul de similarités entre résumés à l'aide de la similarité cosinus.
    Segmentation des articles en clusters thématiques.
    Visualisation des clusters dans un espace 2D réduit par PCA.

Technologies utilisées
Langages et outils principaux :

    Python : Langage de programmation principal.
    Jupyter Notebook : Pour l'analyse et le prototypage.

# Bibliothèques Python :

    Pandas et NumPy : Manipulation et analyse de données.
    Matplotlib et Seaborn : Visualisation de données.
    Scikit-learn : Vectorisation TF-IDF, réduction PCA et clustering K-means.
    NLTK : Traitement du langage naturel (prétraitement des textes).
    Biopython : Extraction de données depuis l'API PubMed.
    ThreadPoolExecutor : Parallélisation des requêtes API.

# Installation
# Prérequis :

    Python 3.7 ou version supérieure.
    Un compte NCBI pour utiliser l'API PubMed (obligatoire pour obtenir une clé d'API).

# Étapes :

    Clonez ce dépôt sur votre machine locale :



Accédez au répertoire du projet :

cd pubmed-analysis

Installez les dépendances nécessaires :

pip install -r requirements.txt

# Configurez votre clé d'API PubMed dans le fichier Python :

    from Bio import Entrez
    Entrez.email = "votre-email@example.com"
    Entrez.api_key = "votre-clé-api"

# Structure du projet


Exécution
# Étape 1 : Extraction des données

Exécutez le script pour récupérer les articles depuis PubMed :

python src/data_extraction.py

# Étape 2 : Nettoyage et prétraitement

Nettoyez les données et appliquez la vectorisation TF-IDF :

python src/preprocessing.py

# Étape 3 : Clustering et visualisation

Appliquez PCA, K-means et visualisez les clusters :

python src/clustering.py

# Résultats

    Statistiques descriptives : Analyse des longueurs de résumés et du nombre d’auteurs.
    Clustering thématique : Segmentation des articles en 5 clusters principaux.
    Visualisation des clusters : Projection des articles dans un espace 2D après réduction PCA.

# Exemple de visualisation :

# Applications potentielles

    Analyse des thématiques dominantes dans un domaine scientifique.
    Regroupement des articles similaires pour faciliter la recherche.
    Extraction des tendances ou des sujets émergents.

# Prochaines étapes

    Ajouter un modèle de topic modeling (LDA) pour identifier les thèmes des clusters.
    Intégrer une interface utilisateur simple pour interagir avec les données.
    Étendre l'analyse à d'autres bases de données scientifiques.

# Auteur

  kobla Legbedje : Etudiant en Data Science passionné par le NLP et les applications en sciences.

# Contact

Pour toute question ou suggestion, n'hésitez pas à me contacter à modestelgk@gmailcom
