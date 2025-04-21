
# Group Analysis - Notebook Guide

## Overview
This Jupyter Notebook performs group-based analysis on functional dependencies (FDs) discovered in structured datasets. It supports data visualization, FD evaluation, and dependency graph interpretation.

---

## How to Use

### 1. Environment
- **Platform**: Jupyter Notebook
- **Language**: Python 3.x
- **Dependencies**:
  - `pandas`
  - `matplotlib`
  - `networkx`
  - `seaborn` (optional for styling)
  - `os`, `json`, `collections`, etc.

Ensure all dependencies are installed in your environment.

---

### 2. Change Dataset

To use your own data:
- **Modify the file paths** at the **beginning of the notebook**, e.g.:

```python
data_path = "/content/drive/MyDrive/your_folder/your_fd_result.csv"
```

- Replace only the path variables — no need to change the logic of the modules.

---

### 3. Run by Module

Since this notebook is modularized by section headings, you can:
- **Click on the Markdown title** of any analysis section (e.g., `## Association Rule`)
- **Run all cells under that section** directly by pressing **Shift+Enter**, or using the “Run” dropdown → “Run selected cell and below”

This allows you to:
- Selectively execute only the steps you need
- Quickly re-run plots or analytics on different datasets without re-executing the full notebook

---

## Notebook Structure

### Data Preparation: Single Column Profiling
- **part1: Cardinalities** – Number of rows, nulls, distinct values, uniqueness
- **part2: Value Distribution** – Histogram plots for numerical features
- **Similarity Metrics**:
  - Levenshtein distance
  - Levenshtein ratio
  - Weighted Dice
  - Dice
  - `thefuzz`-based string matching

---

### Association Rule
- **Top 10 Association Rules**
- **Association Rule Network Graph**
- **Top 10 Rules with Support, Confidence, Leverage, and Conviction**
- **Word Cloud of Most Frequent Items**
- **KMeans Clustering of Rules**

---

### Multi-column FD & Primary Key Detection

#### Visualisation
- Heatmap of FD relationships
- FD network graph
- Barplot of top FD scores
- Confidence vs Coverage scatter plot
- FD source field frequency barplot

#### Checkpoint & Result
- Checkpoint loading / saving
- Main analysis functions

---

### FD & IND Discovery (`fd_ind` Section)
- Find exact FDs
- Find approximate FDs (e.g., error rate = 0.05)
- Find exact INDs
- Find approximate INDs (e.g., error rate = 0.2)
- Inclusion Dependencies with Threshold 0.2
- Main analysis function

---
---

## Notes
- If running on **Google Colab**, make sure your Google Drive is mounted before modifying file paths.
- Results will typically be stored in output folders in the same directory unless otherwise specified.
