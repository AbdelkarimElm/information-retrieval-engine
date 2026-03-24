# Information Retrieval Engine

Moteur de recherche d'information construit dans le cadre d'une compétition Kaggle
(Master Informatique – Université Paris Cité).

## Phase 1 – Retrieval basics
- Exploration et statistiques du corpus (216 041 documents), des requêtes et de la vérité terrain
- Prétraitement : normalisation des nombres, nettoyage, stopwords, stemming
- Modèles lexicaux : TF-IDF et BM25+
- Modèle sémantique : embeddings avec découpage en chunks, visualisation UMAP
- Évaluation : Recall@k, Precision@k, MRR
