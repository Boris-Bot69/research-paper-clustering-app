# 📚 Research Paper Analysis & Clustering App

This project is a **Streamlit-based web application** that allows you to **upload research papers in PDF format**, automatically extract their text, and **analyze semantic similarity and clustering** of the documents using various machine learning techniques.

It’s especially useful for:

* Exploring large sets of academic papers
* Finding related works
* Visualizing thematic clusters
* Running similarity search between documents

---

## 🚀 Features

* 📄 **PDF Text Extraction** using `PyMuPDF`
* 🧠 **Semantic Embedding** using `sentence-transformers` (`all-MiniLM-L6-v2`)
* 🔍 **Paper Similarity Search** (via cosine similarity)
* 🧹 **Clustering Algorithms**:

  * DBSCAN
  * K-Means
  * Spectral Clustering
  * Gaussian Mixture Models (GMM)
  * Agglomerative Clustering
  * OPTICS
* 🕸️ **Graph-Based Visualizations** with NetworkX and Matplotlib
* 🌐 **Interactive UI** via Streamlit

---

## 📂 Directory Structure

```
.
├── app.py                         # Main Streamlit application
├── extract_and_cluster.py        # Functions for clustering, embedding, and PDF parsing
├── papers/                       # Directory to place your PDF files
├── requirements.txt              # Python dependencies
└── README.md                     # This file
```

---

## 🧪 How to Use

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/paper-analysis-app.git
cd paper-analysis-app
```

### 2. Install Dependencies

We recommend using a virtual environment (e.g., `conda` or `venv`):

```bash
pip install -r requirements.txt
```

### 3. Add Your PDFs

Place all your PDF research papers into the `papers/` directory.

### 4. Run the App

```bash
streamlit run app.py
```

---

## 💽 Application Overview

Once launched, you can:

1. Select a **clustering algorithm** from the sidebar
2. Click **"Cluster"** to visualize paper groupings
3. Click **"Find Similar Papers"** to view top 5 semantically closest papers to randomly chosen examples
4. Explore visual graph plots generated via NetworkX

---

## 🧠 Models & Libraries

* **Embeddings**: \[Sen
