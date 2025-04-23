## Analyse de Sentiment — Lab 01 & Lab 02

Ce dossier contient deux notebooks Jupyter consacrés à l’analyse de sentiment sur un jeu de données financières (`finance_sentiment.csv`)

### Lab 01 – Approche Classique
- **Lecture & Préparation des données** : chargement du CSV, nettoyage minimal, découpage train/test (70 %/30 %).
- **Extraction de caractéristiques** : vectorisation texte par Bag-of-Words / TF-IDF.
- **Classification** : modèle **Multinomial Naive Bayes**.
- **Évaluation** : accuracy, matrice de confusion, rapport de classification.

### Lab 02 – Amélioration par Modèles Pré-entraînés
- **Préparation & Split** : mêmes étapes de lecture et découpage que Lab 01.
- **Embeddings contextuels** : utilisation de **BERT** via Hugging Face (`AutoTokenizer` & `AutoModel`) pour générer des vecteurs de phrase.
- **Pipeline de classification** : un réseau **GRU** (Gated Recurrent Unit) entraîné sur ces embeddings.
- **Comparaison des performances** : gains en précision, rappel et F1-score par rapport à la solution classique.

---

Ces deux travaux montrent l’évolution d’un pipeline d’analyse de sentiment, depuis une solution statistique simple jusqu’à une approche profonde exploitant la richesse sémantique de BERT.  
