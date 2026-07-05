# Clustering

In this repo we will have a look at clustering.

## Table of Contents
- [Features](#features)
- [How It Works](#how-it-works)
- [Technology Stack](#technology-stack)
- [Requirements](#requirements)
- [Installation](#installation)
- [Configuration](#configuration)
- [Quick Start](#quick-start)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Development](#development)
- [Limitations](#limitations)
- [License](#license)

## Features

### Data Visualization
- **Matplotlib & Seaborn**: Visualize clustering results and compare different algorithms.

### Machine Learning Algorithms
- **Scikit-Learn**: Implement and evaluate various clustering algorithms like K-Means, DBSCAN, Hierarchical Clustering.
  
### Text Processing
- **NLTK & Gensim**: Perform text clustering using techniques like TF-IDF and Word2Vec.

### Image Processing
- **Rasterio**: Cluster images based on pixel similarity or feature extraction.

## How It Works

The project consists of Jupyter Notebooks that guide you through the process of clustering data. Each notebook focuses on a specific type of clustering (e.g., customer segmentation, image clustering, text clustering).

### Workflow Diagram
```
+-------------------+
| 1_Comparing_Clustering_Algorithms.ipynb |
+-------------------+
          |
          v
+-------------------+
| 2_Clustering_for_Customer_Segmentation.ipynb |
+-------------------+
          |
          v
+-------------------+
| 3_Clustering_Images.ipynb |
+-------------------+
          |
          v
+-------------------+
| 4_Bonus_Clustering_Texts.ipynb |
+-------------------+
```

## Technology Stack

| Technology | Purpose |
|------------|---------|
| Jupyter Notebook | Interactive environment for data analysis and visualization. |
| Matplotlib & Seaborn | Data visualization tools. |
| Pandas | Data manipulation and analysis library. |
| NumPy | Numerical computing library. |
| Scikit-Learn | Machine learning library with clustering algorithms. |
| NLTK & Gensim | Natural language processing and text clustering libraries. |
| Rasterio | Image processing library for reading and writing geospatial raster data. |

## Requirements

- Python 3.11.3
- GDAL (for image processing)

## Installation

### macOS
```bash
make setup
source .venv/bin/activate
```

### WindowsOS
For PowerShell CLI:
```powershell
pyenv local 3.11.3
python -m venv .venv
.venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
pip install -r requirements.txt
```

For Git-bash CLI:
```bash
pyenv local 3.11.3
python -m venv .venv
source .venv/Scripts/activate
python -m pip install --upgrade pip
pip install -r requirements.txt
```

## Configuration

No specific configuration files are required.

## Quick Start

1. Fork the repository.
2. Clone your forked repository to your local machine.
3. Navigate to the project directory and run:
   ```bash
   make setup
   source .venv/bin/activate
   ```
4. Open each Jupyter Notebook in sequence (`1_Comparing_Clustering_Algorithms.ipynb`, `2_Clustering_for_Customer_Segmentation.ipynb`, etc.) to follow along with the clustering tasks.

## Usage

Each notebook provides detailed instructions and code snippets for performing clustering. Here are some example commands:

- **K-Means Clustering**:
  ```python
  from sklearn.cluster import KMeans
  kmeans = KMeans(n_clusters=3)
  kmeans.fit(data)
  ```

- **DBSCAN Clustering**:
  ```python
  from sklearn.cluster import DBSCAN
  dbscan = DBSCAN(eps=0.5, min_samples=10)
  dbscan.fit(data)
  ```

## Project Structure

```
ds-clustering/
├── .github/workflows/
│   ├── REGX_test_import_libraries.sh
│   ├── add_issue_to_done.yml
│   ├── add_issue_todo.yml
│   ├── add_pr_in_progress.yml
│   ├── add_pr_to_done.yml
│   ├── discord-webhook-notify.yml
│   ├── replacement.yml
│   └── workflow-07.yml
├── .gitignore
├── 1_Comparing_Clustering_Algorithms.ipynb
├── 2_Clustering_for_Customer_Segmentation.ipynb
├── 3_Clustering_Images.ipynb
├── 4_Bonus_Clustering_Texts.ipynb
├── Makefile
├── README.md
├── data.zip
├── images/
│   ├── Seville_Spain.jpg
│   ├── dbscan.png
│   ├── seville_clustered.jpg
│   └── seville_new.jpg
└── requirements.txt
```

## Development

The project uses a Makefile for environment setup. Contributions are welcome, but please ensure that any new features or changes are thoroughly tested.

## Limitations

- The project assumes familiarity with Python and machine learning concepts.
- Some notebooks may require additional data preprocessing steps depending on the dataset used.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.