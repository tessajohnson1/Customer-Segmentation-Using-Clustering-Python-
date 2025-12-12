# Customer-Segmentation-Using-Clustering-Python-

# Overview

This project applies K-Means clustering to segment customers based on demographic and behavioral features.
The goal is to help businesses identify customer groups, understand their behavior, and tailor marketing strategies effectively.

This is my second project at Infotach, focusing on end-to-end data preprocessing, EDA, clustering, visualization, and insights reporting.

# Project Objective

•	Segment customers into meaningful groups using K-Means clustering

•	Identify common traits within each cluster

•	Build data-driven marketing recommendations for each customer segment

•	Provide visualizations (EDA, PCA plots, cluster charts) to support insights

# Key Features

✔ Cleaned and preprocessed dataset
✔ Performed EDA (histograms, boxplots, correlations)
✔ Normalized numerical features using StandardScaler
✔ Applied K-Means clustering
✔ Determined optimal number of clusters using:
    • Elbow Method
    • Silhouette Score
✔ Visualized clusters using PCA (2D scatterplot)
✔ Generated insights and marketing recommendations

# Dataset Description

The dataset contains 1,000 customer records with the following attributes:

•	id	Unique customer ID
•	age	Customer age
•	gender	Male/Female
•	income	Annual income
•	spending_score	Engagement / spending indicator
•	membership_years	Loyalty membership duration
•	purchase_frequency	Average monthly purchase count
•	last_purchase_amount	Recent spending amount
•	preferred_category	Product category preference

Categorical features were converted into dummy variables for modeling.

# Tech Stack

•	Python

•	Pandas, NumPy

•	Matplotlib, Seaborn

•	Scikit-learn (StandardScaler, PCA, KMeans)

•	Jupyter Notebook

# Project Workflow
1️⃣ Data Loading & Cleaning

•	Checked missing values

•	Encoded categorical variables

•	Removed inconsistencies

2️⃣ Exploratory Data Analysis (EDA)

•	Age distribution

•	Income distribution

•	Category preferences

•	Correlation heatmaps

•	Spending score patterns

3️⃣ Feature Scaling

•	Applied StandardScaler to numerical columns for fair distance calculation in K-Means.

4️⃣ Clustering

•	Used Elbow Method and Silhouette Score to determine optimal k = 4

•	Trained final K-Means model and assigned cluster labels

5️⃣ Visualization

•	PCA scatterplot color-coded by cluster

•	Cluster-level boxplots & distribution charts

6️⃣ Cluster Profiling

•	Generated mean values per cluster to analyze:

•	Spending behavior

•	Shopping categories

•	Income differences

•	Purchase frequency

7️⃣ Marketing Recommendations

•	Cluster-based strategies such as:

•	Upselling & cross-selling for high-value customers

•	Discounts for cost-sensitive groups

•	Loyalty rewards for frequent buyers

# Key Insights
⭐ Cluster 0

Younger customers with moderate spending

Prefer electronics

Strategy: Cross-sell accessories, targeted digital ads

⭐ Cluster 1

Older customers, lower spending

Prefer groceries

Strategy: Loyalty discounts, retention programs

⭐ Cluster 2

High-income & high-spending customers

Frequent buyers

Strategy: Premium offers, VIP membership

⭐ Cluster 3

Moderate income, high purchase frequency

Prefer home & garden

Strategy: Seasonal promotions, bundle offers

# Results

Successfully identified 4 distinct customer segments

Improved understanding of customer behavior

Designed actionable marketing plans

# Limitations

Dataset is synthetic — real-world data may require deeper cleaning

K-Means assumes spherical clusters

PCA reduces dimensionality but may lose variance

# Future Enhancements

Try advanced clustering (DBSCAN, Hierarchical Clustering)

Build a customer lifetime value (CLV) prediction model

Deploy segmentation using a dashboard (Streamlit/PowerBI)

📁 Repository Structure
│
├── infotach.ipynb               # Main analysis notebook
├── cleaned_dataset.csv          # Preprocessed dataset
├── images/                      # Plots & visualizations
│   ├── pca_clusters.png
│   ├── elbow_method.png
│   ├── silhouette_scores.png
│   └── ...
├── README.md                    # Project documentation
└── requirements.txt             # Dependencies
