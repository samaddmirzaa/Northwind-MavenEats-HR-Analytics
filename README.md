# Unsupervised Machine Learning

This repo contains all the notebooks I worked through for an unsupervised machine learning course, covering everything from data prep and clustering through to dimensionality reduction and recommender systems. Each topic has a lecture notebook, a set of practice assignments, and (for a few of them) a hands-on project with a real business scenario.

The datasets are in the `data` folder (uploaded as a zip). 

---

## What's Covered

**01 - Data Prep**
Getting data into the right shape for unsupervised modeling. Row granularity, group-by aggregations, scaling, and encoding.

**02 - Clustering**
K-Means from scratch, inertia plots to choose the right K, hierarchical clustering, and DBSCAN. Covers how to interpret and compare cluster assignments, including using silhouette scores to evaluate which model actually makes sense.

**03 - Anomaly Detection**
Using Isolation Forests and DBSCAN to flag unusual records in a dataset. Includes visualizing anomalies and tuning the sensitivity of the model.

**04 - Dimensionality Reduction**
PCA for compressing features and understanding which ones carry the most variance. t-SNE for visualizing high-dimensional clusters in 2D. Also covers layering cluster labels onto dimensionality reduction plots to see how well your segments hold up visually.

**05 - Recommenders**
Content-based filtering using cosine similarity, and collaborative filtering using TruncatedSVD. Ends with a demo of a hybrid recommender that combines both approaches.

---

## Projects

### Clustering Clients — Northwind Traders
*Notebook: `02_clustering_project.ipynb`*

Northwind Traders is a wholesale distributor supplying gourmet food products to restaurants, cafes, and specialty retailers. Using their yearly client report (channel, region, and spend by product category), the goal is to segment clients into meaningful groups using three different clustering techniques, evaluate them, and predict which segment a new client would fall into.

![Brief](briefs/Brief_1.png)

### Recommending Restaurants — MavenEats
*Notebook: `05_recommender_project.ipynb`*

MavenEats is a restaurant review website. The task is to build two recommenders: one that suggests five restaurants for a user's homepage based on their past ratings, and one that surfaces five similar restaurants on each restaurant's detail page.

![Brief](briefs/Brief_2.png)

### Final Project — HR Analytics
*Notebook: `06_final_project.ipynb`*

An end-to-end unsupervised learning project for an HR Analytics team at a mid-sized software company. The company wants to reduce attrition, so the job is to segment employees using clustering, visualize those clusters with dimensionality reduction, explore what makes each group distinct, and make concrete recommendations for improving retention in each one.

![Brief](briefs/Brief_3.png)

---

## Repo Structure

```
├── data/                          # All datasets 
├── 01_data_prep.ipynb
├── 01_data_prep_assignments.ipynb
├── 02_clustering.ipynb
├── 02_clustering_assignments.ipynb
├── 02_clustering_project.ipynb
├── 03_anomaly_detection.ipynb
├── 03_anomaly_detection_assignments.ipynb
├── 04_dimensionality_reduction.ipynb
├── 04_dimensionality_reduction_assignments.ipynb
├── 05_recommenders.ipynb
├── 05_recommenders_assignments.ipynb
├── 05_recommender_project.ipynb
└── 06_final_project.ipynb
```

## Requirements

All notebooks use standard Python data science libraries. You can install everything you need with:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn scipy
```
