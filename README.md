# Unsupervised Clustering and Differential Expression Analysis of Lung scRNA-seq Data
 📄 ** Full Report:** [View here](Final_Project_Report.pdf)
## Introduction
This project explores single-cell RNA sequencing (scRNA-seq) data from lung tissue in healthy mice to identify distinct cell populations and the genes that drive their separation. Using unsupervised learning techniques, the goal is to uncover structure in high-dimensional biological data and better understand how different lung cell types are organized and function.

## Technologies
- **Python**  
- **NumPy**, **Pandas**  
- **Scikit-learn** (PCA, K-means clustering)  
- **Matplotlib**, **Seaborn**  
- **Google Colab** (notebook environement) 


## Features
- Dimensionality reduction using PCA to visualize high-dimensional gene expression data  
- K-means clustering to identify distinct cell populations  
- Differential expression analysis to identify cluster-specific marker genes  
- Biological interpretation of clusters (endothelial, immune, stromal, epithelial, etc.)  
- Validation using annotated Tabula Muris dataset  

## How I Built It
1. Loaded scRNA-seq lung dataset (Tabula Muris)  
2. Performed preprocessing and filtering  
3. Applied PCA to reduce dimensionality  
4. Used K-means clustering to group cells into 6 clusters  
5. Conducted differential expression analysis to identify marker genes per cluster  
6. Interpreted clusters biologically based on gene expression patterns  
7. Validated results using annotated cell-type data  

## Results
- Identified 6 distinct clusters of lung cells  
- Clear separation observed for several clusters in PCA space, indicating distinct cell types  
- Found biologically meaningful gene markers:
  - Endothelial cells (e.g., Cldn5, Esam)  
  - Immune cells (e.g., Srgn, Cd53)  
  - Alveolar epithelial cells (e.g., Sftpc, Sftpa1)  
  - Stromal / mesenchymal cells  
- Observed overlapping clusters suggesting transitional or related cell states  
- Validation showed general agreement with known cell-type annotations, with some expected discrepancies  


## What I Learned
- How to apply unsupervised learning techniques to high-dimensional biological data  
- The importance of dimensionality reduction in interpreting complex datasets  
- How clustering results depend heavily on preprocessing and model assumptions  
- That biological systems often exist on a spectrum (continuous cell states), not strict clusters  
- Limitations of linear methods like PCA for capturing complex biological variation  


## How It Could Be Improved
- Use non-linear dimensionality reduction methods (e.g., UMAP, t-SNE) for better separation  
- Apply more advanced clustering methods (e.g., hierarchical clustering, Leiden algorithm)  
- Improve preprocessing to reduce noise and sparsity in scRNA-seq data  
- Incorporate additional datasets or experimental validation  
- Explore deeper differential expression analysis across more genes  

*Developed as part of BioE 149 (Computational Biology) at UC Berkeley*
