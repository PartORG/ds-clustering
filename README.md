# Clustering

In this repo we will have a look at clustering.

## Task

Please work in pairs through all the notebooks in this particular order:

1. [Comparing Clustering Algorithms](1_Comparing_Clustering_Algorithms.ipynb)
2. [Clustering for Customer Segmentation](2_Clustering_for_Customer_Segmentation.ipynb)
3. [Image Clustering](3_Clustering_Images.ipynb)


## Environment

Use the [requirements](requirements.txt) file in this repo to create a new environment.
You can either run `make setup` (make sure to activate the environment after the installation) or the following commands:

```BASH
pyenv local 3.11.3
python -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install -r requirements.txt
```

If You encounter errors related to GDAL try:

```BASH
brew install GDAL
pip install -r requirements.txt
```
