# Stock Market Clustering using K-Means and Fractal Clustering

## Overview

This project implements stock market clustering using **K-Means Clustering** and extends it with a **Fractal (Recursive Hierarchical) Clustering** approach for improved stock segmentation and analysis.

The implementation is based on the Medium article:

- https://medium.com/uptick-blog/stock-picks-using-k-means-clustering-4330c6c4e8de

The project analyzes stock behavior using:
- Annual Returns
- Volatility (Risk)
- Recursive clustering techniques
- Cluster visualization and evaluation

---

## Features

### Implemented Techniques

- Data preprocessing and normalization
- Feature engineering using:
  - Mean Returns
  - Variance / Volatility
- K-Means clustering
- Elbow Method for optimal K selection
- Recursive Fractal Clustering
- Cluster visualization
- Correlation heatmaps
- Dendrogram analysis
- Cluster-based stock selection
- CSV export of clustered stocks

---

## Project Structure

```bash
.
├── Stock_Clustering_PrachiGupta.ipynb
├── stock_clustering_outputs/
└── README.md
```

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- SciPy
- yFinance

---

## Clustering Workflow

### 1. Data Collection
Stock market data is collected using Yahoo Finance (`yfinance`).

### 2. Feature Extraction
The following features are calculated:
- Average Returns
- Variance
- Standard Deviation
- Risk Metrics

### 3. K-Means Clustering
Stocks are grouped into clusters based on similar market behavior.

### 4. Fractal Clustering
Each cluster is recursively subdivided into smaller clusters for fine-grained analysis.

### 5. Visualization
The project generates:
- Scatter plots
- Elbow curve
- Heatmaps
- Dendrograms

---

## Fractal Clustering Concept

Fractal clustering recursively applies clustering within clusters.

Example:

```text
Cluster 0
 ├── Subcluster 0A
 ├── Subcluster 0B
      ├── Subcluster 0B-1
      └── Subcluster 0B-2
```

This helps identify:
- Highly correlated stock groups
- Sector-like behavior
- Hidden market patterns

---

## Results

The notebook successfully:
- Identifies stock groups with similar risk-return behavior
- Performs recursive cluster refinement
- Visualizes cluster separation
- Generates interpretable clustering outputs

---

## How to Run

### Run Jupyter Notebook

```bash
jupyter notebook
```

Open:

```bash
Stock_Clustering_PrachiGupta.ipynb
```

---

## Sample Output

The notebook produces:
- Cluster scatter plots
- Cluster statistics
- Heatmaps
- Dendrograms
- Recursive cluster outputs

---

## Learning Outcomes

This project demonstrates:
- Unsupervised Machine Learning
- Financial Data Analysis
- Clustering Algorithms
- Recursive Pattern Discovery
- Data Visualization

---

## Future Improvements

- DBSCAN implementation
- Gaussian Mixture Models
- Portfolio optimization
- Deep learning embeddings
- Real-time stock analysis

---

## Author

**Prachi Gupta**

Graduate Student — San Jose State University

---

## License

This project is for academic and educational purposes.
