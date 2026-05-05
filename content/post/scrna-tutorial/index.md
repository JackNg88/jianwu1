---
title: "Getting started with single-cell RNA-seq analysis in R"
date: 2024-03-01
tags:
  - scRNA-seq
  - R
  - Tutorial
  - Bioinformatics
summary: "A practical introduction to single-cell RNA-seq data analysis using Seurat in R, covering QC, clustering, and visualization."
---

Single-cell RNA sequencing (scRNA-seq) has revolutionized our understanding of cellular heterogeneity. In this post, I share my workflow for analysing scRNA-seq data using **Seurat** in R.

## 1. Loading data

```r
library(Seurat)
data <- Read10X(data.dir = "path/to/10x/output/")
seurat_obj <- CreateSeuratObject(counts = data, min.cells = 3, min.features = 200)
```

## 2. Quality Control

```r
seurat_obj[["percent.mt"]] <- PercentageFeatureSet(seurat_obj, pattern = "^MT-")
VlnPlot(seurat_obj, features = c("nFeature_RNA", "nCount_RNA", "percent.mt"))
seurat_obj <- subset(seurat_obj, subset = nFeature_RNA > 200 & percent.mt < 20)
```

## 3. Normalization & Clustering

```r
seurat_obj <- NormalizeData(seurat_obj)
seurat_obj <- FindVariableFeatures(seurat_obj, nfeatures = 2000)
seurat_obj <- ScaleData(seurat_obj)
seurat_obj <- RunPCA(seurat_obj)
seurat_obj <- FindNeighbors(seurat_obj, dims = 1:20)
seurat_obj <- FindClusters(seurat_obj, resolution = 0.5)
seurat_obj <- RunUMAP(seurat_obj, dims = 1:20)
DimPlot(seurat_obj, reduction = "umap")
```

More tutorials coming soon!
