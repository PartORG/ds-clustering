# Clustering Algorithms and Techniques

A comprehensive guide to clustering algorithms, customer segmentation, image clustering, and text clustering using Jupyter Notebooks.

[![GitHub Actions](https://github.com/PartORG/ds-clustering/actions/workflows/workflow-07.yml/badge.svg?branch=main&event=workflow_dispatch)](https://github.com/PartORG/ds-clustering/actions/workflows/workflow-07.yml)
[![License](https://img.shields.io/github/license/PartORG/ds-clustering)](LICENSE)

## Introduction

Clustering is a fundamental technique in data analysis and machine learning, used to group similar data points together. This repository provides a detailed exploration of various clustering algorithms, customer segmentation, image clustering, and text clustering using Jupyter Notebooks.

### Primary Workflow

1. **Comparing Clustering Algorithms**: Understand the strengths and weaknesses of different clustering techniques.
2. **Customer Segmentation Clustering**: Apply clustering to segment customers based on their behavior and preferences.
3. **Image Clustering**: Group images with similar visual features together.
4. **Text Clustering (Bonus)**: Explore advanced clustering methods for text data.

### Main Advantages

- **Educational Value**: Learn practical applications of clustering algorithms through hands-on examples.
- **Versatility**: Apply clustering techniques to various domains such as customer segmentation, image analysis, and text mining.
- **Automation**: Use GitHub workflows for automated testing and notifications.

## Features

### Clustering Algorithms Comparison

Explore different clustering algorithms like K-Means, Hierarchical Clustering, DBSCAN, and more. Understand their use cases and performance characteristics.

### Customer Segmentation Clustering

Learn how to segment customers based on their behavior and preferences using clustering techniques. This helps in targeted marketing and personalized customer experiences.

### Image Clustering

Group images with similar visual features together. This is useful for image retrieval systems, content-based filtering, and more.

### Text Clustering (Bonus)

Explore advanced clustering methods for text data. This includes techniques like Latent Dirichlet Allocation (LDA) and Word2Vec for text segmentation.

## How It Works

The repository is primarily written in Jupyter Notebooks. The Makefile automates the installation of Python and required packages using pyenv and pip. GitHub workflows handle various automation tasks such as testing library imports and notifying via Discord.

### Technology Stack

| Technology | Purpose |
|------------|---------|
| **Jupyter Notebook** | Interactive environment for data analysis and visualization. |
| **Python** | Programming language for data manipulation and machine learning. |
| **pyenv** | Python version manager to manage multiple Python versions. |
| **pip** | Package installer for Python packages. |
| **scikit-learn** | Machine learning library for clustering algorithms. |
| **matplotlib** & **seaborn** | Libraries for data visualization. |
| **pandas** & **numpy** | Data manipulation and numerical computing libraries. |
| **nltk** & **gensim** | Natural language processing libraries. |
| **rasterio** | Library for reading and writing geospatial raster data. |
| **scipy** | Scientific computing library with advanced mathematical functions. |

## Requirements

- Python 3.11.3
- GDAL (for image clustering)

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
pip install --upgrade pip
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
3. Run `make setup` to set up the environment.
4. Activate the virtual environment and run the Jupyter Notebooks in the specified order.

## Usage

Run the Jupyter Notebooks in the following order:

1. [Comparing Clustering Algorithms](1_Comparing_Clustering_Algorithms.ipynb)
2. [Clustering for Customer Segmentation](2_Clustering_for_Customer_Segmentation.ipynb)
3. [Image Clustering](3_Clustering_Images.ipynb)
4. [BONUS: Text Clustering](4_Bonus_Clustering_Texts.ipynb)

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

The development workflow involves using Jupyter Notebooks for prototyping and testing. GitHub workflows handle automated testing and notifications.

## Testing

GitHub workflows are used for automated testing of library imports and notifications via Discord.

## Limitations

- Limited support for older versions of Python.
- No support for real-time clustering applications.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.