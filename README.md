# DBSCAN - Clustering with Densities
### App Link
- https://dbscan-clustering-with-densities.streamlit.app/
---
### What is DBSCAN?
- DBSCAN means **Density-Based Spatial Clustering of Applications with Noise**.
- It is a **clustering algorithm** that groups data based on how **close** and **dense** the points are.
- It is helpful when we don’t know how many groups (clusters) are there in advance.
- **Real-Life Example:** Imagine a park where people are standing.
  - If 5–6 people are standing **close together**, they form a **group** (cluster).
  - If someone is standing **far away**, they are **ignored** (outlier).
- If points are tightly packed, DBSCAN makes a group. If a point is alone, DBSCAN marks it as noise.
---
### Why use DBSCAN?
- We **don't need to give number of clusters** like KMeans
- It works well for **irregular shapes**. It can also find **outliers** in our data.
---
### Some Key Terms and their Meaning
- **eps:** How close 2 points should be to be considered neighbors.
- **min_samples:** How many nearby points are needed to form a group.
- **Core Point:** Has enough neighbors (forms the cluster).
- **Border Point:** Close to a core point but doesn't have enough points.
- **Noise:** Too far from others, not in any cluster.
---
### Output
`Labels: [0 0 0 1 1 -1]`
- First 3 points → Cluster 0 (label **`0`**)
- Next 2 points → Cluster 1 (label **`1`**)
- Last point → Too far, marked as noise (label **`-1`**)

  **Visual Explanation:**
```
● ● ●        ← Cluster 0  
         

                ● ●     ← Cluster 1  

                            ●    ← Outlier / Noise
```

---
### Some Important Points
- DBSCAN finds clusters **automatically** - No need to specify count.
- It is **great at finding outliers** in messy data.
- It works even when clusters are not round (unlike KMeans).
---
