arXiv [WIP]
==============================

### arXiv metadata analysis project
arXiv is the pre-print server. Pre-print means the paper before published to a scientific journal. Scientists are also upload their papers to arXiv.
The papers on arXiv aren't peer-reviewed, so we can read the paper as soon as it published and free.

## Dataset
The dataset is from Kaggle.
https://www.kaggle.com/Cornell-University/arxiv

### Data structure
id: ArXiv ID (can be used to access the paper, see below)  
submitter: Who submitted the paper  
authors: Authors of the paper  
title: Title of the paper  
comments: Additional info, such as number of pages and figures  
journal-ref: Information about the journal the paper was published in  
doi: https://www.doi.org (Digital Object Identifier)  
abstract: The abstract of the paper  
categories: Categories / tags in the ArXiv system  
versions: A version history  

The number of entries is over 1.7 million.
So I used the part of it here.

### Categories 

## Notebooks
The notebooks are from kaggle notebook.

[Category trend](https://github.com/tomokr/arxiv/blob/master/notebooks/1-tomokr-arxiv-categories-trend.ipynb) ... Analyzing categories trend  
[Abstract to category](https://github.com/tomokr/arxiv/blob/master/notebooks/2-tomokr-arxiv-abstract-nlp.ipynb)...Predicting category from the abstract using spaCy  
[Title to category](https://github.com/tomokr/arxiv/blob/master/notebooks/3-tomokr-arxiv-title-nlp-tensorflow.ipynb)...Predicting category from the title using TensorFlow  

## Category trend


## Future works
- Dask : to handle the entire dataset


Project Organization
------------

    ├── LICENSE
    ├── Makefile           <- Makefile with commands like `make data` or `make train`
    ├── README.md          <- The top-level README for developers using this project.
    ├── data
    │   ├── external       <- Data from third party sources.
    │   ├── interim        <- Intermediate data that has been transformed.
    │   ├── processed      <- The final, canonical data sets for modeling.
    │   └── raw            <- The original, immutable data dump.
    │
    ├── docs               <- A default Sphinx project; see sphinx-doc.org for details
    │
    ├── models             <- Trained and serialized models, model predictions, or model summaries
    │
    ├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
    │                         the creator's initials, and a short `-` delimited description, e.g.
    │                         `1.0-jqp-initial-data-exploration`.
    │
    ├── references         <- Data dictionaries, manuals, and all other explanatory materials.
    │
    ├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
    │   └── figures        <- Generated graphics and figures to be used in reporting
    │
    ├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
    │                         generated with `pip freeze > requirements.txt`
    │
    ├── setup.py           <- makes project pip installable (pip install -e .) so src can be imported
    ├── src                <- Source code for use in this project.
    │   ├── __init__.py    <- Makes src a Python module
    │   │
    │   ├── data           <- Scripts to download or generate data
    │   │   └── make_dataset.py
    │   │
    │   ├── features       <- Scripts to turn raw data into features for modeling
    │   │   └── build_features.py
    │   │
    │   ├── models         <- Scripts to train models and then use trained models to make
    │   │   │                 predictions
    │   │   ├── predict_model.py
    │   │   └── train_model.py
    │   │
    │   └── visualization  <- Scripts to create exploratory and results oriented visualizations
    │       └── visualize.py
    │
    └── tox.ini            <- tox file with settings for running tox; see tox.readthedocs.io


--------

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>
