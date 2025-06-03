# DBSCAN - Clustering with Densities
### App Link
- https://dbscan-clustering-with-densities.streamlit.app/
---
### What is DBSCAN?
- DBSCAN means **Density-Based Spatial Clustering of Applications with Noise**.
- It is a **clustering algorithm** that groups data based on how **close** and **dense** the points are.
- It is helpful when we don’t know how many groups (clusters) are there in advance.
- DBSCAN works well for **irregular shapes** and can find **outliers** in our data. There's **no need to give number of clusters** like KMeans.
---
### How DBSCAN works
- Output : `[ 0  0  0  1  1 -1 ]`
- First 3 points → Cluster 0 (label **`0`**)
- Next 2 points → Cluster 1 (label **`1`**)
- Last point → Too far, marked as noise (label **`-1`**)
- DBSCAN finds clusters **automatically** - no need to specify count.
---
