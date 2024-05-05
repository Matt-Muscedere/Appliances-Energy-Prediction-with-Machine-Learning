# Appliances Energy Production
This repository is the holding place of all data and subsequent trained models from a publicly available dataset found [here](https://archive.ics.uci.edu/dataset/374/appliances+energy+prediction). The ML algorithms used will be regression based.

*These notebooks have been developed for Project 1 of COMP-4730 (Advanced AI Concepts I) at the University of Windsor, Fall 2023.*

# How To Run
**These instructions assume Python and Jupyter have both been properly installed!**

When attempting to run any Jupyter Notebook file, first ensure that the appropriate libraries have been installed. This can be done by running:
```
pip install -r requirements.txt
```
This will automatically install all Python libraries listed within the `requirements.txt` file. 

The algorithms run off of the [`DataEnergyClean.csv`](https://github.com/CadenQ/comp4730-p1/blob/main/data/DataEnergyClean.csv) dataset, which is a cleaned version of [`energydata_complete.csv`](https://github.com/CadenQ/comp4730-p1/blob/main/data/energydata_complete.csv) (cleaned in [`data_prep.ipynb`](https://github.com/CadenQ/comp4730-p1/blob/main/data_prep.ipynb)).

## Inside of [`reg_algos.ipynb`](https://github.com/CadenQ/comp4730-p1/blob/main/reg_algos.ipynb)
To see how your own algorithm might pit up against the included algorithms, make sure your algorithm is imported. Then, simply scroll down to the `models` dictionary, and insert your model with a given name. Then simply run all cells (make sure you installed all libraries from `requirements.txt`) and observe the results!

# Files
The following lays out details on what each file contains.

## Datasets
- [`data`](https://github.com/CadenQ/comp4730-p1/tree/main/data)
    - [`DataEnergyClean.csv`](https://github.com/CadenQ/comp4730-p1/blob/main/data/DataEnergyClean.csv) contains the cleaned dataset used for the algorithms of this project. It contains 19735 rows and 25 columns.
    - [`energydata_complete.csv`](https://github.com/CadenQ/comp4730-p1/blob/main/data/energydata_complete.csv) contains the original dataset provided by UCI. It contains 19735 rows and 29 columns.

## Data Preparation
- [`data_prep.ipynb`](https://github.com/CadenQ/comp4730-p1/blob/main/data_prep.ipynb) handled all data cleaning to be processed by sklearn's algorithms. The main change was reducing the dataset from 29 columns to 25.

## Algorithms
- [`grid_search_code.ipynb`](https://github.com/CadenQ/comp4730-p1/blob/main/grid_search_code.ipynb) was used to optimize every algorithm. 
- [`reg_algos.ipynb`](https://github.com/CadenQ/comp4730-p1/blob/main/reg_algos.ipynb) contains all the algorithms used to analyze the dataset and compute the results. All graphs created are included in this file.