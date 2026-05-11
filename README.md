# Information Retrieval Engine

Moteur de recherche d'information construit dans le cadre d'une compétition Kaggle
(projet de groupe, Master Informatique – Université Paris Cité, 2025/2026).

## Phase 1 – Retrieval basics
- Exploration et statistiques du corpus (216 041 documents), des requêtes et de la vérité terrain
- Prétraitement : normalisation des nombres, nettoyage, stopwords, stemming
- Modèles lexicaux : TF-IDF et BM25+
- Modèle sémantique : embeddings avec découpage en chunks, visualisation UMAP
- Évaluation : Recall@k, Precision@k, MRR

## Phase 2 – Classification et reranking
- Classification des documents et requêtes en 5 catégories (Logistic Regression, SVM)
- Courbes d'apprentissage, matrices de confusion, évaluation sur holdout
- Re-chunking et ré-embedding avec un modèle BGE-base-en-v1.5 fine-tuné
- Reranking combinant similarité sémantique, catégorie prédite et tags

## Exécution
Le notebook a été conçu pour Google Colab (GPU recommandé).

1. Définir les variables d'environnement `KAGGLE_USERNAME` et `KAGGLE_KEY`
2. Installer les dépendances : `pip install -r requirements.txt`
3. Ouvrir `information_retrieval_engine.ipynb` et exécuter les cellules dans l'ordre
