# Mnist_tsne_clustering
📌 Project Overview

This project demonstrates unsupervised learning on handwritten digit images using
t-SNE (t-Distributed Stochastic Neighbor Embedding) for dimensionality reduction and
K-Means clustering for grouping similar digits.
The main objective is to visualize how high-dimensional image data can be meaningfully
represented and clustered in a 2D space.

📊 Dataset

Dataset used: sklearn.datasets.load_digits()

Total samples: 1,797

Image size: 8 × 8 grayscale

Each image is flattened into a numerical feature vector before processing.

True digit labels (0–9) are used only for evaluation, not for training.

🧠 Methodology
1. Data Preprocessing

Load handwritten digit images

Flatten image pixels into numerical vectors

2. Dimensionality Reduction (t-SNE)

High-dimensional image data is reduced to 2D

t-SNE preserves local similarity, making it ideal for visualization

Used only for visualization, not prediction

3. Clustering (K-Means)

K-Means is applied on the 2D embeddings

Number of clusters (k) is set to 10

Each digit is assigned to a cluster based on similarity

4. Visualization

Interactive 2D scatter plot created using Plotly

Each point represents a digit image

Points are color-coded by cluster

Hovering over a point shows:

True digit label

Assigned cluster

📈 Cluster Analysis

The following metrics are used to evaluate clustering quality:

Cluster size (number of samples per cluster)

Dominant digit in each cluster

Clustering accuracy (by mapping clusters to most frequent digit)

Silhouette score to measure cluster separation

Misclassified digits visualization to analyze overlaps between similar digits

📌 Results & Observations

Clear cluster separation is visible in the 2D space

Most clusters align well with true digit labels

Some overlap occurs between visually similar digits (e.g., 3 and 5)

t-SNE effectively reveals structure in handwritten digit data

Clustering quality metrics indicate meaningful unsupervised grouping

⚙️ Technologies Used

Python

NumPy

Pandas

scikit-learn

Plotly

Matplotlib
