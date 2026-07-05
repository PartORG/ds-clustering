# ds-clustering

Explore clustering algorithms and techniques with interactive Jupyter Notebooks.

## Requirements

To run this project, you need the following dependencies:

- Python 3.11.3
- jupyterlab==3.6.3
- matplotlib==3.7.1
- seaborn==0.12.2
- pandas==2.0.1
- numpy==1.24.3
- scikit-learn==1.2.2
- nltk==3.8.1
- rasterio==1.3.7
- gensim==4.3.1
- scipy==1.12.0

## Installation

### macOS

To set up your environment on macOS, run the following commands:

```bash
make setup
```

After that, activate your environment with:

```bash
source .venv/bin/activate
```

### WindowsOS

For WindowsOS, use either PowerShell or Git-bash CLI to install the required packages:

**PowerShell:**

```powershell
pyenv local 3.11.3
python -m venv .venv
.venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
pip install -r requirements.txt
```

**Git-bash:**

```bash
pyenv local 3.11.3
python -m venv .venv
source .venv/Scripts/activate
python -m pip install --upgrade pip
pip install -r requirements.txt
```

If you encounter an error when trying to run `pip install --upgrade pip`, try using:

```bash
python.exe -m pip install --upgrade pip
```

## Usage

Run the project by executing the following entry points:

1. [Comparing Clustering Algorithms](1_Comparing_Clustering_Algorithms.ipynb)
2. [Clustering for Customer Segmentation](2_Clustering_for_Customer_Segmentation.ipynb)
3. [Image Clustering](3_Clustering_Images.ipynb)
4. [BONUS: Text Clustering](4_Bonus_Clustering_Texts.ipynb)

Each notebook provides a detailed exploration of clustering techniques and their applications.