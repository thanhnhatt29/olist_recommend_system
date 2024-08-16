# Olist Recommendation System

## Introduction
This project builds a recommendation system for the Olist online sales platform using data from Kaggle. The recommendation system is built using Python in combination with Spark through PySpark.

## Project Structure
1. code: This directory contains Jupyter notebooks for different steps of the project

2. data: This directory contains data from kaggle, clean data and data for modeling

3. images: This directory contains images and charts generated during the analysis and modeling process.

4. proposal, milestone, report are directories used for presentations and store documents during the project execution. 

## Steps
### 1. Data Cleaning
Notebook: [`code/1data_cleaning.ipynb`](code/1data_cleaning.ipynb)

This notebook perform data cleaning steps on the raw CSV files and store the cleaned data in the [`data/clean_data`](data/clean_data) folder.

### 2. Exploratory Data Analysis (EDA)
Notebook: [`code/2EDA.ipynb`](code/2EDA.ipynb)

This notebook perform exploratory data analysis (EDA) to better understand the data and identify important features.

### 3. Building Recommendation Model using Spark ALS
Notebook: [`code/3spark_ALS.ipynb`](code/3spark_ALS.ipynb)

This notebook use the Alternating Least Squares (ALS) algorithm from Spark to build the recommendation model.

### 4. Recommendation Function
Notebook: [`code/4Recommend_function.ipynb`](code/4Recommend_function.ipynb)

This notebook build recommendation functions based on the trained model.

## System Requirements
- Conda
- PySpark
- Jupyter Notebook
- Spark cluster (in a simple way, download Spark and export some variables to .bashrc)

## Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/thanhnhatt29/olist_recommend_system.git
    cd olist_recommend_system
    ```

2. Install the required packages:
    ```bash
    conda env create --name sparkML --file=spark_environment.yaml

    conda activate sparkML
    ```

3. Start Jupyter Notebook:
    ```bash
    jupyter notebook
    ```

4. Open and run the notebooks in the [`code`](code) folder.

## Data
The data used in this project is sourced from the [Kaggle Olist dataset](https://www.kaggle.com/olistbr/brazilian-ecommerce).

## Results
The analysis stored in [`report`](report) folder and model results are stored in the [`code/model`](code/model) folder.
