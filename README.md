
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
data_path = "/content/drive/MyDrive/your_folder/your_fd_result.json"
```

- Replace only the path variables — no need to change the logic of the modules.

---

### 3. Run by Module

Since this notebook is modularized by section headings, you can:
- **Click on the Markdown title** of any analysis section (e.g., `## Step 2: FD Visualization`)
- **Run all cells under that section** directly by pressing **Shift+Enter**, or using the “Run” dropdown → “Run selected cell and below”

This allows you to:
- Selectively execute only the steps you need
- Quickly re-run plots or analytics on different datasets without re-executing the full notebook

---

## Notebook Structure

| Section Title                     | Functionality                              |
|----------------------------------|--------------------------------------------|
| **Step 1: Load and Preprocess**      | Reads FD data from path                    |
| **Step 2: Field Frequency**          | Plots bar chart of field usage             |
| **Step 3: FD Network Graph**         | Visualizes FD connections using networkx   |
| **Step 4: Importance Scoring**       | Ranks FDs by strength or consistency       |
| **Step 5: Heatmap + Redundancy**     | Shows pairwise field dependencies          |
| **Step 6: Confidence & Complexity**  | Analyzes simplicity vs reliability of FDs  |

---

## Notes
- If running on **Google Colab**, make sure your Google Drive is mounted before modifying file paths.
- Results will typically be stored in output folders in the same directory unless otherwise specified.
