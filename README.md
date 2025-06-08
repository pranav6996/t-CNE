# 🌀 t-SNE Visualization of 3D Blobs

This project explores dimensionality reduction using **t-SNE (t-Distributed Stochastic Neighbor Embedding)** and plots both 3D and 2D visualizations of clustered data for better understanding of how data structure can be simplified and visualized.

---

## 🌟 What I Learned

- How to generate synthetic data using `make_blobs()` with custom cluster centers and standard deviations.
- How high-dimensional data (3D in this case) can be visualized in 2D using t-SNE.
- The importance of **standardizing data** using `StandardScaler()` before applying t-SNE.
- What parameters like `perplexity` and `max_iter` mean in t-SNE:
  - `perplexity`: kinda like the number of close neighbors t-SNE considers.
  - `max_iter`: how long t-SNE optimizes the embedding (more = better quality but slower).
- Visual tricks using matplotlib and plotly to make data visualization aesthetic and easy to read.

---

## 📊 What I Plotted

### ✅ 3D Scatter Plot
- Used `plotly` to plot a 3D scatter of 4 synthetic blobs (clusters).
- Each point was colored by its original cluster label.

### ✅ 2D t-SNE Projection
- Applied `StandardScaler` to normalize the 3D data.
- Reduced it to 2D using `TSNE()` from sklearn.
- Used `matplotlib` to plot the 2D projection with color-coded clusters.
- Added customizations like:
  - `edgecolor='k'` for sexy dot outlines
  - `cmap='viridis'` for pretty color gradients
  - `alpha` for transparent markers
